# funcstoragevnet
ARM Template for deploying azure function app with storage account with vnet firewall rule in place   
Turns out this works, as long as the storage account file share is also explicitly created

This template also contains an NSG for blocking outbound traffic from function, except to needed resources.   
For some reason the Storage account rule also needs port 80 to work, although this is not listed as a required port anywhere
