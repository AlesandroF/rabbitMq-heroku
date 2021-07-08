FROM mcr.microsoft.com/dotnet/aspnet:5.0

COPY bin/Release/net5.0/ App/
WORKDIR /App
ENTRYPOINT ["dotnet", "RabbitHeroku.dll"]

ENV COMPlus_EnableDiagnostics=0

CMD ASPNETCORE_URLS=http://*:$PORT dotnet RabbitHeroku.dll