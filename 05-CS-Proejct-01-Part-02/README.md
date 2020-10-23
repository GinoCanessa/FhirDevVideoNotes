# Getting Started in C# (.Net Core)

This session is Part 2 of building a basic .Net Core CLI application in C# to connect to an open FHIR server.

## Video Link

[C# Tutorial 01 Part 02](https://youtu.be/aP6DRYH-qOI)

## Notes

* Quick overview of git branches
* Quick review of what we've done
* Coding
  * Add local server
  * Refactor (move from main to ListPatients)
  * Create a `Patient`
  * Read specific patient
  * Delete a `Patient`
  * Update a `Patient`
  * Create multiple `Patients`

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
