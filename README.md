# Azure GO SDK Example 

This program gets a list of all resource groups in a subscription and list VMs in every resource group. 

## Prerequisities 

Program assumes you do have an Azure account, Azure CLI and a working go installation with dep installed. 

## Preparing

Before using or changing the code, run:

```dep ensure``` 

Create service principal file:

```az ad sp create-for-rbac --sdk-auth > my.auth```

And export path to the authorizer:

```export AZURE_AUTH_LOCATION=my.auth```

## Running

Just run with `go run main.go` 

## Licence 

Dariusz Dwornikowski, Nordcloud, MIT
