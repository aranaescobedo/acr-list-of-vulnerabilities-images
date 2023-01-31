# acr-list-of-vulnerabilities-images

This kusto query provides a list of images stored in your Azure Container Registry (ACR) that have vulnerabilities. The query is based on a sample provided by [Microsoft docs](https://learn.microsoft.com/en-us/azure/container-registry/resource-graph-samples?tabs=azure-cli#sample-queries) and has been enhanced to include additional columns to help identify the relevant pod and image tag.

## Requirements
- You need to have Read permissions on the ACR.

## Usage

Simply copy and paste the query into the Azure Resource Graph query tool and run the query. The results will show all vulnerable images along with their respective pod and image tag for the specified ACR. 

If desired, the results can be filtered to display vulnerabilities for a specific ACR and/or namespace by replacing "ADD-ACR-NAME" with the desired ACR's name and "ADD-NAMESPACE-NAME" with the desired namespace name, respectively.

## Limitations

- This query is based on data from the Azure Container Registry and may not reflect the latest security vulnerabilities. It is recommended to regularly check for and apply updates to your images to ensure the highest level of security.

- Please note that it could take up to two days for a deleted image to be removed from the results of this query.

## Disclaimer

This query is provided as-is and is not officially supported by Microsoft. Use at your own discretion.
