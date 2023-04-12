FROM mcr.microsoft.com/dotnet/aspnet:6.0 AS base
WORKDIR /app

EXPOSE 443

COPY published/ .

ENV MONGO_URL=mongodb://mymongo:27017
ENV MONGO_INITDB_DATABASE=BookStore


ENTRYPOINT ["dotnet", "DotNetCoreMongoDbAPI.dll"]


