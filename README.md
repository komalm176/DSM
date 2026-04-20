# DSM

az rest --method post --uri "https://management.azure.com/subscriptions/c7fd7250-bb98-4ce0-bf7e-deba223c1151/resourceGroups/rg-eus2-datalake-dev-01/providers/Microsoft.Web/sites/logic-eus2-dev-filescheduler-01/hostruntime/runtime/webhooks/workflow/api/management/workflows/email-ingestion-workflow/triggers/Poll_Inbox_Every_5_Minutes/listCallbackUrl?api-version=2024-04-01"

az webapp config appsettings list --name logic-eus2-dev-filescheduler-01 --resource-group rg-eus2-datalake-dev-01 --query "[?name=='WEBSITE_RUN_FROM_PACKAGE']"

Get-ChildItem -Path "C:\Users\KomalMehetre\source\repos\DSMTest\LogicApp\email-ingestion-logic" -Recurse

Add-Type -Assembly System.IO.Compression.FileSystem
[System.IO.Compression.ZipFile]::OpenRead("C:\Users\KomalMehetre\source\repos\DSMTest\LogicApp\deploy.zip").Entries | Select-Object FullName