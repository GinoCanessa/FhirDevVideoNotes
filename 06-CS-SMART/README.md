# SMART with C#

This session begins the exploration of using SMART FHIR servers from C#.

## Video Links

* [SMART C# With a Local Server Part 01](https://youtu.be/lrlQjpGdKI0)
* [SMART C# With a Local Server Part 02](https://youtu.be/250UNIdndeY)
* [SMART C# With a Local Server Part 03](https://youtu.be/_WNBRxvNORg)
* [SMART C# With a Local Server Part 04](https://youtu.be/3CWpn3FtpX8)
* [SMART C# With a Local Server Part 05](https://youtu.be/L0FefJZrOVY)

## Notes

* Part 1: Setup
  * Project goals
      * Access a SMART FHIR Server
      * Use a local web server for redirection
  * Create repo
  * Install NuGet Packages
* Part 2: Discovering SMART
  * Via FHIR metadata
  * Via .well-known
* Part 3: Setting up a webserver
  * Basic setup
  * Determining port
  * Running in the background
* Part 4: Completing a flow
  * Launch authorization
  * Receive code
  * Exchange code for Token
* Part 5: Using a Token
  * Parsing the SMART return
  * Using a Token with a FHIRClient

## Tools

* [Basic Tools](https://github.com/GinoCanessa/FhirDevVideoNotes/tree/main/04-CS-Project-01#tools)

## FHIR Links

* [Patient](http://hl7.org/fhir/patient.html)
* [SMART App Launch Framework](http://www.hl7.org/fhir/smart-app-launch/)

## Other Links

* [SMART App Launcher](https://launch.smarthealthit.org/)
* [Loopback Interface Redirection](https://tools.ietf.org/html/rfc8252#section-7.3)

## NuGet Packages

* [Hl7.Fhir.R4](https://www.nuget.org/packages/Hl7.Fhir.R4/)
  * `dotnet add package Hl7.Fhir.R4 --version 1.9.0`
* [Microsoft.AspNetCore.App](https://www.nuget.org/packages/Microsoft.AspNetCore.App/)
  * `dotnet add package Microsoft.AspNetCore.App --version 2.2.8`
* [Microsoft.AspNetCore.Cors](https://www.nuget.org/packages/Microsoft.AspNetCore.Cors/)
  * `dotnet add package Microsoft.AspNetCore.Cors --version 2.2.0`
* [Microsoft.AspNetCore.Razor.Design](https://www.nuget.org/packages/Microsoft.AspNetCore.Razor.Design/)
  * `dotnet add package Microsoft.AspNetCore.Razor.Design --version 2.2.0`
* [Microsoft.Extensions.Configuration](https://www.nuget.org/packages/Microsoft.Extensions.Configuration/)
  * `dotnet add package Microsoft.Extensions.Configuration --version 3.1.9`
* [Microsoft.Extensions.Configuration.EnvironmentVariables](https://www.nuget.org/packages/Microsoft.Extensions.Configuration.EnvironmentVariables/)
  * `dotnet add package Microsoft.Extensions.Configuration.EnvironmentVariables --version 3.1.9`
* [Microsoft.Extensions.Configuration.Json](https://www.nuget.org/packages/Microsoft.Extensions.Configuration.Json/)
  * `dotnet add package Microsoft.Extensions.Configuration.Json --version 3.1.9`
* [System.CommandLine.DragonFruit](https://www.nuget.org/packages/System.CommandLine.DragonFruit/)
  * `dotnet add package System.CommandLine.DragonFruit --version 0.3.0-alpha.20371.2`
