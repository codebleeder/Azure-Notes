cloud notes 

72-4e3f7399-accessing-and-using-the-azure-cloud-sh

commands
az group list 
az storage account list 
az vm list

az vm create `
--name LabVM `
--resource-group 72-4e3f7399-accessing-and-using-the-azure-cloud-sh `
--image UbuntuLTS `
--admin-username azureuser `
--generate-ssh-keys

// the keys generated in the above command are in temp storage. You need to move to a permanent storage. 

------------
powershell commands 
Get-AzResourceGroup
Get-AzStorageAccount
Get-AzVM
Get-AzResource | ft //ft = format 

// remove vm 
Remove-AzVM -Name LabVM -ResourceGroupName 72-4e3f7399-accessing-and-using-the-azure-cloud-sh