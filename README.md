# Store.V1 - E-Commerce API (Clean Architecture)
<div align="center">
  
**⚠️ READ THIS FIRST ⚠️**

*The repository is named `Store.V1`, but this is **NOT version 1.0** of the software.*  
*This is the complete, production-ready e-commerce API (v2.0+).*  
*The "V1" is legacy naming and does not indicate version number.*

</div>
A robust, scalable RESTful API for e-commerce store management built with **.NET Core**, **SQL Server**, and **Clean Architecture** principles.

## 🏗️ Clean Architecture Overview

This project follows **Clean Architecture** (also known as Onion Architecture) to achieve separation of concerns, maintainability, and testability.
<table>
<tr>
<td align="center" style="background:#e8f5e9; padding:20px; border-radius:10px">
<b>🟢 PRESENTATION LAYER</b><br>
API / Controllers
</td>
</tr>
<tr>
<td align="center" style="background:#e1f5fe; padding:20px; border-radius:10px">
<b>🔵 APPLICATION LAYER</b><br>
DTOs / Services / Mapping
</td>
</tr>
<tr>
<td align="center" style="background:#f3e5f5; padding:20px; border-radius:10px">
<b>🟣 DOMAIN LAYER (Core)</b><br>
Entities / Interfaces 
</td>
</tr>
<tr>
<td align="center" style="background:#fff3e0; padding:20px; border-radius:10px">
<b>🟠 INFRASTRUCTURE LAYER</b><br>
Data/DbContext / Repositories
</td>
</tr>
</table>

 ### Dependency Rule
Dependencies point inward. The inner layers (Domain) have no dependencies on outer layers (Infrastructure, Presentation).

## 🚀 Technologies Used

- **.NET Core 9** - Backend framework
- **Clean Architecture** - Separation of concerns
- **Entity Framework Core** - ORM for database operations
- **SQL Server** - Primary database
- **ASP.NET Core Web API** - RESTful API
- **JWT Authentication** - Secure authentication
- **Swagger/OpenAPI** - API documentation
- **AutoMapper** - Object mapping
- **Visual Studio 2022** - IDE


## 📋 Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) with:
  - ASP.NET and web development workload
  - .NET desktop development workload
- [.NET Core SDK 9.0 ](https://dotnet.microsoft.com/download)
- [SQL Server](https://www.microsoft.com/en-us/sql-server/sql-server-downloads) (Express/Developer)
- [Git](https://git-scm.com/)
## 📦 NuGet Packages Used

### Core & Database
| Package | Version | Description |
|---------|---------|-------------|
| [Microsoft.EntityFrameworkCore](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore) | 9.0.0 | Core Entity Framework library |
| [Microsoft.EntityFrameworkCore.SqlServer](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.SqlServer) | 9.0.0 | SQL Server provider for EF Core |
| [Microsoft.EntityFrameworkCore.Design](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Design) | 9.0.0 | Design-time tools for EF Core migrations |
| [Microsoft.EntityFrameworkCore.Tools](https://www.nuget.org/packages/Microsoft.EntityFrameworkCore.Tools) | 9.0.0 | EF Core PowerShell commands |

### Authentication & Security
| Package | Version | Description |
|---------|---------|-------------|
| [Microsoft.AspNetCore.Authentication.JwtBearer](https://www.nuget.org/packages/Microsoft.AspNetCore.Authentication.JwtBearer) | 9.0.0 | JWT Bearer authentication for ASP.NET Core |

### Mapping
| Package | Version | Description |
|---------|---------|-------------|
| [AutoMapper](https://www.nuget.org/packages/AutoMapper) | 15.1.3 | Object-object mapper |
| [AutoMapper.Extensions.Microsoft.DependencyInjection](https://www.nuget.org/packages/AutoMapper.Extensions.Microsoft.DependencyInjection) | 11.0.0 | AutoMapper DI integration |

### API & Logging
| Package | Version | Description |
|---------|---------|-------------|
| [Microsoft.AspNetCore.OpenApi](https://www.nuget.org/packages/Microsoft.AspNetCore.OpenApi) | 9.0.14 | OpenAPI support for ASP.NET Core |
| [Microsoft.Extensions.Logging.Abstractions](https://www.nuget.org/packages/Microsoft.Extensions.Logging.Abstractions) | 10.0.6 | Logging abstractions |
## 🔧 Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/farissyria/Store.V1.git
cd Store.V1
