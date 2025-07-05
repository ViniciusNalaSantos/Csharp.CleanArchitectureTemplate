# Clean Architecture .NET Solution Template

## 🌟 Overview
A modern, clean architecture template for .NET applications following domain-driven design principles and best practices. This template provides a solid foundation for building scalable, maintainable, and testable applications.

## 🏗️ Architecture Overview

```
CleanArchitectureDemo/
├── Domain/             # Enterprise/domain entities & business rules
├── Application/        # Business logic & use cases
├── Infrastructure/     # External concerns (database, file systems, etc.)
├── WebApi/            # User interface & API endpoints
└── UnitTests/         # Unit tests for all layers
```

### Layer Details

#### 🎯 Domain Layer
- Contains enterprise/business logic
- Entities
- Value Objects
- Domain Events
- Interfaces
- Business Rules
- No dependencies on other layers

#### 🔄 Application Layer
- Contains application logic
- Implements use cases
- DTOs
- Interfaces
- Service implementations
- Dependencies: Domain layer

#### 🛠️ Infrastructure Layer
- Implementation of interfaces from Domain/Application layers
- Database contexts
- Repositories implementations
- External service implementations
- Dependencies: Domain and Application layers

#### 🌐 WebApi Layer
- API Controllers
- API Models
- Middleware
- Dependencies: Application layer

## 🚀 Getting Started

### Prerequisites
- .NET 8.0 SDK or later
- Visual Studio 2022 or VS Code
- SQL Server (optional)

### Installation

1. Clone the repository
```bash
git clone https://github.com/ViniciusNalaSantos/Csharp.CleanArchitectureTemplate.git
cd CleanArchitectureTemplate
```

2. Build the solution
```bash
dotnet build
```

3. Run the tests
```bash
dotnet test
```

4. Run the application
```bash
cd ProjectName.WebApi
dotnet run
```

## 📝 Project Structure

```
CleanArchitecture/
├── Domain/
│   ├── Entities/
│   └── Interfaces/
│
├── Application/
│   ├── DTOs/
│   ├── Interfaces/
│   └── Services/
│
├── Infrastructure/
│   ├── DatabaseContext/
│   └── Repositories/
│
├── WebApi/
│   ├── Controllers/
│   └── Program.cs
│
└── UnitTests/
    ├── Domain/
    ├── Application/
    └── Infrastructure/
```

## 🙏 Acknowledgments

- Clean Architecture by Robert C. Martin
- Microsoft .NET Documentation
- Entity Framework Core Documentation
- xUnit Documentation

## Give a Star! :star:

If you like or are using this project to learn or start your solution, please give it a star. Thanks!
