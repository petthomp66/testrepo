# ABS (Albertsons) Azure Vnet Onstruct Migration to cAPIC
-------------------------------------------------------------
This script read Azure's Vnet objects, maps these cAPIC ojects and creates those cAPIC objects on the cAPIC running virtual machine.

--------------------------------------------------------------
Requirements:
-----------------------------------------------
------------------------------------
* Python 3.8
* Azure CLI LIbrary (Pip install azure-cli)
* Cisco ACI SDK (pyACI SDK Library)

Python version
-----
Script was developed using python version 3.8

Azure CLI
---
Azure CLI is used for:

1. Authentication. Detailes for Azure CLI are noted:
https://docs.microsoft.com/en-us/cli/azure/install-azure-cli

Once the Azure CLI is installed, run az login to authenticate or az login --help to view other authentication options.

2. Collection of Azure configurations:

Azure CLI uses Python and can be used with Windows, MAC or Linux:

Install Azure libraries via: 

$Pip install azure-cli

Cisco ACI SDK (pyACI SDK Library)
-----------

1.	Install Library:

Download meta data from the controller:

https://<APIC controller IP address>/doc/jsonmeta/aci-meta.json

Copy Meta file to a local directy and configure within python script:

Example:

   apic = Node('https://{}'.format(args.ip), aciMetaFilePath="/root/scripts/aci-meta.json")
   
   
Note: A copy of the file is in the repo with name: "aci-meta.json"

-----------------------
Usage:

$








