# FHIR via (manual) HTTP

## Video Link

[FHIR via HTTP](https://www.youtube.com/watch?v=eBAQYMT2KtM)

## Notes

* [FHIR Interactions (REST)](http://hl7.org/fhir/http.html)
* [Public Test Servers](https://confluence.hl7.org/display/FHIR/Public+Test+Servers)
* [FHIR R4 Examples](http://hl7.org/fhir/hl7.fhir.r4.examples.tgz)

* Interaction overview
  * Instance vs Type vs System
  * URL format
* [Bundles](http://hl7.org/fhir/bundle.html)
* [Search](http://hl7.org/fhir/search.html)

## Commands

* curl example - get CapabilityStatement
```
curl --location --request GET 'http://hapi.fhir.org/baseR4/metadata' --header 'Accept: application/fhir+json'
```