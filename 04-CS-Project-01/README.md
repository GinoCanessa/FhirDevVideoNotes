# Getting Started in C# (.Net Core)

This session covers building a basic .Net Core CLI application in C# to connect to an open FHIR server.

## Video Link

(Recording in progress...)

## Notes

* Short overview of development environment
* Project description
  * .Net Core CLI
    * Cross Platform
    * No UI components to 'get in the way'
    * Focus on FHIR and interactions
  * Functionality
    * Get a list of `Patient` resources on the server
    * Search for a specific `Patient` resource
    * Get related `Encounter` resources for the `Patient`

## Tools

* [.NET Core](https://dotnet.microsoft.com/download/dotnet-core)
  * [C# XML Doc Comments](https://marketplace.visualstudio.com/items?itemName=k--kato.docomment)
* [Visual Studio Code](https://code.visualstudio.com/)
* [git](https://git-scm.com/)
* [Windows Terminal](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701)
  * Scott Hanselman - [Pretty Terminal](https://www.hanselman.com/blog/how-to-make-a-pretty-prompt-in-windows-terminal-with-powerline-nerd-fonts-cascadia-code-wsl-and-ohmyposh)

## FHIR Resources

* [Patient](http://hl7.org/fhir/patient.html)
* [Encounter](http://hl7.org/fhir/encounter.html)
* [Search](https://www.hl7.org/fhir/search.html)
  * [Include and RevInclude](https://www.hl7.org/fhir/search.html#include)
* [Patient Compartment](https://www.hl7.org/fhir/compartmentdefinition-patient.html)

## NuGet Packages
* [Hl7.Fhir.R4](https://www.nuget.org/packages/Hl7.Fhir.R4/)

## Commands

* 