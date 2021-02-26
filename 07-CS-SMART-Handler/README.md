# SMART with C#

This set of videos covers building a C# SMART application with a custom URI scheme.

## Video Links

* [SMART C# With a custom URI scheme Part 01](https://youtu.be/APzpXFTZk6E)

## Notes

* Part 1: Setup
  * Project goals
      * Access a SMART FHIR Server
      * Use a custom URI scheme for redirection
  * Create repo
  * Install NuGet Packages
  * Configure URI scheme in Windows (registry)


## Tools

* [Basic Tools](https://github.com/GinoCanessa/FhirDevVideoNotes/tree/main/04-CS-Project-01#tools)

## FHIR Links

* [SMART App Launch Framework](http://www.hl7.org/fhir/smart-app-launch/)

## Other Links

* Apple
  * [Defining a Custom URL Scheme for Your App](https://developer.apple.com/documentation/xcode/allowing_apps_and_websites_to_link_to_your_content/defining_a_custom_url_scheme_for_your_app)
* Linux
  * [Stack Overflow - xdg](https://unix.stackexchange.com/questions/497146/create-a-custom-url-protocol-handler)
* Windows
  * [Registering an Application to a URI Scheme](https://docs.microsoft.com/en-us/previous-versions/windows/internet-explorer/ie-developer/platform-apis/aa767914(v=vs.85)?redirectedfrom=MSDN)

## NuGet Packages

* [Microsoft.Win32.Registry](https://www.nuget.org/packages/Microsoft.Win32.Registry/)
  * `dotnet add package Microsoft.Win32.Registry --version 6.0.0-preview.1.21102.12`
* [System.CommandLine.DragonFruit](https://www.nuget.org/packages/System.CommandLine.DragonFruit/)
  * `dotnet add package System.CommandLine.DragonFruit --version 0.3.0-alpha.20574.7`
