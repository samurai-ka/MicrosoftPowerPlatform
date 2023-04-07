# Microsoft Power Platform

## Connectors

### Files to Include

An Open API 2.0 swagger definition, an API properties file, and a README.md.

### API Definition (Swagger) File

The API definition, also known as the swagger, describes the API for the custom connector using the OpenAPI specification.

For further details, see the [apiDefinition.swagger.json](schemas/apiDefinition.swagger.schema.json) JSON schema.

### API Properties File

The API properties file contains some properties for the custom connector. These properties are not part of the API definition. It contains information such as the brand color, authentication information, etc. A typical API properties file looks like the following:

```json
{
  "properties": {
    "capabilities": [],
    "connectionParameters": {
      "api_key": {
        "type": "securestring",
        "uiDefinition": {
          "constraints": {
            "clearText": false,
            "required": "true",
            "tabIndex": 2
          },
          "description": "The KEY for this API",
          "displayName": "KEY",
          "tooltip": "Provide your KEY"
        }
      }
    },
    "iconBrandColor": "#007EE6",
    "policyTemplateInstances": [
      {
        "title": "MyPolicy",
        "templateId": "setqueryparameter",
        "parameters": {
            "x-ms-apimTemplateParameter.name": "queryParameterName",
            "x-ms-apimTemplateParameter.value": "queryParameterValue",
            "x-ms-apimTemplateParameter.existsAction": "override"
        }
      }
    ]    
  }
}
```

For further details, see the [apiProperties.json](schemas/paconn-apiProperties.schema.json) JSON schema.

### README.md

README.md file for the connector includes a description for the connector, any prerequisite you may need to setup the connector. It includes instructions on how to use the connector and api, how to get credentials, supported operations, known issues and limitations, etc.
