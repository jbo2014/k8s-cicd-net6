FROM maven2.it.volvo.net:18443/nvs-dotnet-60-ubi8:latest
WORKDIR /app

EXPOSE 9090
ENV ASPNETCORE_URLS="http://+:9090"
ENV ASPNETCORE_ENVIRONMENT="Development"

COPY bin/Release/net6.0/publish/ .
ENTRYPOINT ["dotnet", "dotnetapi.dll"]