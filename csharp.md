
## C# Notes ##

dotnet add package MySql.EntityFrameworkCore
dotnet add package MySql.Data
dotnet add package MySql.Data --version 8.3.0
dotnet add package Microsoft.EntityFrameworkCore.Tools
dotnet add package MySql.Data.EntityFrameworkCore.Design

dotnet restore

echo $PATH

dotnet ef dbcontext scaffold "server=127.0.0.1;port=3306;user=user;password=password;database=db" MySql.EntityFrameworkCore -o Models -f\


