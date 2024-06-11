FROM cgr.dev/chainguard/dotnet-sdk:latest AS build
COPY --chown=nonroot:nonroot . /source
WORKDIR /source
RUN dotnet publish --use-current-runtime --self-contained false -o Release

FROM cgr.dev/chainguard/dotnet-runtime:latest AS final
WORKDIR /
COPY --from=build source .
ENTRYPOINT ["dotnet", "Release/HelloWorldApp.dll"]
