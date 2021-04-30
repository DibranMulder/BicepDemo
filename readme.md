# Bicep demo

```bash
az login
```

```bash
az account set --subscription "Visual Studio Enterprise"
```

```bash
az group create --name testdibranbicep --location "West Europe"
```

```bash
az deployment group create --name addmodule --resource-group testdibranbicep --template-file azuredeploy.bicep --parameters storagePrefix=store storageSKU=Standard_LRS webAppName=demoapp
```