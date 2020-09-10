# Azure CLI

az policy definition create --name 'enforce-resourceGroup-tags'  --display-name 'Enforce tags costCenter and businessUnit' --description 'Enforce tags costCenter and businessUnit' --rules 'https://raw.githubusercontent.com/eBerdnA/azure-policies/master/ResourceGroup/enforce-resourceGroup-tags/azurepolicy.rules.json' --mode All

az policy assignment create --name <assignmentname> --scope <scope> --policy "enforce-resourceGroup-tags"


az policy assignment create --name "demo-"enforce-resourceGroup-tags"" --scope "/subscriptions/a188c6fe-a61f-4ead-8753-67d8702bc161" --policy "enforce-resourceGroup-tags"

# Sources

* [az policy definition](https://docs.microsoft.com/en-us/cli/azure/policy/definition?view=azure-cli-latest)
* [az policy assignment](https://docs.microsoft.com/en-us/cli/azure/policy/assignment?view=azure-cli-latest)