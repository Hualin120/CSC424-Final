FROM mcr.microsoft.com/dotnet/sdk:10.0 AS builder



WORKDIR /src



COPY backend/backend.csproj ./

RUN dotnet restore



COPY backend/ ./



RUN dotnet publish -c Release -o /app/publish --no-restore



FROM mcr.microsoft.com/dotnet/aspnet:10.0



WORKDIR /app



COPY --from=builder /app/publish .



EXPOSE 8080



ENTRYPOINT ["dotnet", "backend.dll"]

