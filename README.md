# nomis-claim-schema-vocab

> Repository for Nomis credential schema definitions and vocabularies.
>

Repository: [https://github.com/Nomis-cc/nomis-iden3](https://github.com/Nomis-cc/nomis-iden3)

### General description:

This repository contains JSON-LD and JSON schemas for Nomis Iden3 Credentials.
At the current stage, the **nomisScore-v1** data model utilizes W3C Verifiable Credential Model but has some additional defined fields. In the future, it can be fully adapted to the W3C Verifiable Credential standard.

The repository structure is following:

1. credentials

   The folder contains vocabulary definitions for Nomis claim structure and vocabulary.
   For example, field *score* is defined in [NomisScore.md](credentials/NomisScore.md) vocabulary file and resolved to link [https://github.com/Nomis-cc/nomis-iden3/blob/main/credentials/NomisScore.md#score](https://github.com/Nomis-cc/nomis-iden3/blob/main/credentials/NomisScore.md#score) that gives information about the field: description, type, example.

   - Example of NomisCredential:

       ```json
      TODO
       ```

2. schemas

   - JSON

     JSON schemas define the validation rules for claim content (using JSON standard)
     and also specifies the order of fields to fill claim slots (according to claim specification). For that *Index* and *Value* custom fields are used. Implementors *must* use these fields.

   - JSON-LD

     JSON-LD schema allows to provide both - association with data vocabulary and claim slot specification. It doesn't confront with JSON, but extending the possibilities. This create an opportunity to exchange documents in machine readable format with document normalization and linked data structures and human readable by providing needed vocabulary.