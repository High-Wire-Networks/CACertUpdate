https://github.com/High-Wire-Networks/CACertUpdate
# CACertUpdate
Scripts to update TLS log agents
This update is only required for agents sending logs thru TLS . It does not affect servers using local log collector over UDP.

Windows:
Please use the script provided thru your software distribution tool in your environment to replace the certificate and restart the nxlog service. If not using a software distribution tool , right click on the PowerShell script and run locally on device/s as administrator.

- Fluency-NXLogWindowsCertSwap.ps1


Linux:
Run the script below with sudo user privileges. Ensure the file has permissions to execute by using chmod command.

- Fluency-rsyslogbashCACertSwap.sh
- Fluency-syslogngbashcertswap.sh

Firewall:
Upload the new certificate and remove the old certificate from the certificate store and restart the syslog services .
