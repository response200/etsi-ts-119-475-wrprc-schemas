# ETSI TS 119 475 Wallet-Relying Party Registration Certificate schemas

This repository contains JSON schemas for Wallet-Relying Party Registration Certificates (WRPRCs). WRPRCs are JWTs or CWTs with defined header areas (JOSE Header or COSE Header) and defined payloads (JWS Payload or CWT payload). The JSON schemas are based on the requirements, mappings, classes, multiplicity values and types presented in [ETSI TS 119 475](https://portal.etsi.org/webapp/WorkProgram/Report_WorkItem.asp?WKI_ID=69585) standard. The JSON schemas themselves comply with [JSON Schema](https://json-schema.org/draft/2020-12/json-schema-core) and [JSON Schema Validation](https://json-schema.org/draft/2020-12/json-schema-validation) specifications.

The JSON schemas in this repository describe the data structure of and can be used to validate the JOSE Header and the JWS Payload of a WRPRC in JWT format. The schemas, and JSON Schemas in general, cannot be used to validate WRPRCs in CWT format.

## Repository structure

ETSI TS 119 475 is a versioned standard and this repository reflects that. The schemas and examples are organised in directories whose names match with the standard version they are compatible with (“version directories”). Each version directory contains schemas of the WRPRC header area and the WRPRC payload, and examples of header areas and payloads. When run through a JSON Schema validator an example of a header area or a payload in a certain version directory should validate against the header area or payload schema within the same version directory.

Version directories might contain notes in a README.md file with explanations of the known limitations or issues, if any, in the schemas, examples or in the standard version itself.

The `aspirational-2025-12-05` directory  contains versions of the schemas and examples which are based on my comments on version 1.1.1 of the standard and that were delivered to ETSI on 2025-12-05. The schemas and the examples in the directory describe the WRPRC header area and the WRPRC payload in the form they would have, if all my suggested data structure changes were accepted by ETSI.

## Feedback and contributions

All feedback, corrections and contributions are welcome. Those can be given in the form of issues and pull requests in this repository or by contacting me directly via eg. e-mail.

## Licence

[BSD 3-Clause](LICENCE.md). Authored by Joel Posti.
