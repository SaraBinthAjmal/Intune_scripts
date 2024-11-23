# Intune scripts for Endpoint

## Prerequisites
1.	Remote Management:
    o	Ensure WinRM is enabled on the endpoints.
    o	Configure firewall rules to allow remote management.
2.	PowerShell Modules:
    o	Install PSWindowsUpdate on endpoints for update management.
3.	Administrator Rights:
    o	Run the script with administrative privileges.

##Explanation
1.	Endpoint List: Replace $endpoints with your endpoint names or IP addresses.
2.	Credential Security: The script uses Get-Credential for secure remote authentication.
3.	Get-SystemInfo Function: Retrieves system information using WMI.
4.	Install-Updates Function: Uses the Install-WindowsUpdate cmdlet (from the PSWindowsUpdate module) to install updates and reboot if necessary.
5.	Invoke-Command: Executes scripts remotely on the specified endpoints.

