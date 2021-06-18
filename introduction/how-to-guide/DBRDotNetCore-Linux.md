# .Net core Barcode Reader SDK

## Environment

- DBR version: 8.1.2
- DotNet version: 3.1.407
- Linux release: Ubuntu 16.04

## Installation

1. Dynamsoft.DotNet.Barcode
Please [contact us](https://www.dynamsoft.com/company/contact/) to get the latest DBR DotNet library. 
2. Dynamsoft Barcode Reader SDK
You can download the latest DBR library via [this](https://www.dynamsoft.com/barcode-reader/programming/c?download=true) page.

**For the SDK used in this article, please use [this](http://tst.dynamsoft.com/temp/DotNetCoreDbr.zip) link to download both DotNet and DBR library.**

## Coding

### Create project

```shell
mkdir TestDbrDotCore
cd TestDbrDotCore
dotnet new console
```

### Write a barcode reader application in Program.cs

You could refer to .Net user guide [here](https://www.dynamsoft.com/barcode-reader/programming/dotnet/user-guide.html?ver=latest).

### Modify TestDbrDotCore.csproj

```html
<Project Sdk="Microsoft.NET.Sdk">
  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>netcoreapp3.1</TargetFramework>
  </PropertyGroup>
  <ItemGroup>
   <Reference Include="DynamsoftCommon">
         <HintPath>DynamsoftCommon.dll</HintPath>
   </Reference>
   <Reference Include="Dynamsoft.BarcodeReader">
         <HintPath>Dynamsoft.BarcodeReader.dll</HintPath>
   </Reference>
  </ItemGroup>
</Project>
```

## Run your Project

### Copy dbr library

After downloaded the DBR package, uncompress the file and follow the below steps:

```shell
cp DynamsoftBarcodeReader/Lib/Linux/* /usr/lib
```

### Copy the .Net core library to the project

```shell
cp DynamsoftCommon.dll Dynamsoft.BarcodeReader.dll /Your path to/TestDbrDotCore
```

## Run your project

```shell
dotnet restore
dotnet build
dotnet run
```
