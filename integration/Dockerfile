FROM microsoft/dotnet:2-sdk
WORKDIR /integration

COPY integration/integration.csproj ./integration/
RUN dotnet restore integration/integration.csproj

COPY . .
ENTRYPOINT ["dotnet", "test"]
