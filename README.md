dotnet new webapi -n ProductsApi

dotnet dev-certs https --trust

docker-compose up -d
# => http://localhost:5050/

#
dotnet add package Npgsql.EntityFrameworkCore.PostgreSQL
dotnet tool install --global dotnet-ef
dotnet add package Microsoft.EntityFrameworkCore.Design

dotnet ef migrations add InitialMigration
dotnet ef database update
