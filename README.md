# azure-arm-template-custom-vmss
An Azure ARM Template with: 
- a custom base image
- additional metrics for autoscaling
- application insights with alert rule
- firewall
- loadbalancing

# Usage:
- open the **parameters.json** file and edit *scaleset_name*, *ssh-key*, *ssh_firewall_ip* and *alert_emails*
- then:
```
PS> .\deploy.ps1 -subscriptionId <SUBSCRIPTION-ID> -resourceGroupName <RG-NAME> -resourceGroupLocation <LOCATION> <DEPLOYMENT-NAME> [-debug]
```