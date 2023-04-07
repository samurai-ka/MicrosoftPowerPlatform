# Microsoft Power Platform

## Connectors

A Power Platform connector is a proxy or a wrapper around an API that allows the underlying service to talk to Microsoft Power Automate, Microsoft Power Apps, and Azure Logic Apps. It provides a way for users to connect their accounts and leverage a set of prebuilt actions and triggers to build their apps and workflows.

### In this repository

- [X] **Mastodon** connector
  
  This connector lets you interact with the [Mastodon microblogging](https://joinmastodon.org/) platform.

## Folder structure

### Files to Include

An Open API 2.0 swagger definition, an API properties file, and a README.md.

### API Definition (Swagger) File

The API definition, also known as the swagger, describes the API for the custom connector using the OpenAPI specification.

For further details, see the [apiDefinition.swagger.json](schemas/apiDefinition.swagger.schema.json) JSON schema.

### API Properties File

The API properties file contains some properties for the custom connector. These properties are not part of the API definition. It contains information such as the brand color, authentication information, etc.
For further details, see the [apiProperties.json](schemas/paconn-apiProperties.schema.json) JSON schema.

### README.md

README.md file for the connector includes a description for the connector, any prerequisite you may need to setup the connector. It includes instructions on how to use the connector and api, how to get credentials, supported operations, known issues and limitations, etc.

## Learn more

To learn more about the Power Platform visit the [Power Platform and Azure Logic Apps connectors documentation](https://learn.microsoft.com/en-us/connectors/) site.
