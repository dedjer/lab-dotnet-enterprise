# lab-dotnet-enterprise

Fully featured enterprise ready .NET Core API 

## Description

This is a .NET Core API project built following Ken Berg's enterprse folder structure.

## .NET Requirements

### Option 1: Executable

- Windows - https://learn.microsoft.com/en-us/dotnet/core/install/windows?tabs=net60
- Mac - https://learn.microsoft.com/en-us/dotnet/core/install/macos

### Option 2: Package Manager

- Windows - choco install dotnet -y && choco install dotnet-sdk
- Mac - brew install dotnet


## Liquibase Requirements

### Option 1: Executable

- Windows/Mac - https://www.liquibase.org/download

### Option 2: Package Manager

- Windows - choco install liquibase
- Mac - brew install liquibase

## Manual Project Setup - If you don't feel like cloning this repo

```bash
mkdir src
mkdir src\Company.Product.Feature
cd src
dotnet new sln --name Company.Product
dotnet new webapi -o .\Company.Product.Feature\
dotnet sln add Company.Product.Feature
dotnet dev-certs https --trust
```
