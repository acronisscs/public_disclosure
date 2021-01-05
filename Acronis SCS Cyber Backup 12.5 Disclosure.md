# Acronis Cyber Backup 12.5 SCS Hardened Edition Caveats

Acronis Cyber Backup 12.5 SCS Hardened Edition must be installed per the provided instructions in order to run in fully DoDin APL, Common Criteria, and FIPS 140-2 compliant opertation. The following items should be noted to ensure the desired functionality of the product with regards to a certified environment:
 - RHEL6/Centos6 do not support OS keyring usage, therefore master secrets only have file protections instead of OS keyring protections. 
 - CPUs must support RDRAND in order to be fully FIPS 140-2 compliant. RDRAND provides a high quality documented entropy source for the product. 
 - Properly issued and signed x509 SSL certificates are required to be installed by the user, per the product user guide. 
 - Syslog must be utilized with the product and per our guidance, NXLog can be installed in order to forward appropriate logs. Installation and setup instructions are provided with the product user guide and KB.
 
During installation of the Acronis Cyber Backup 12.5 SCS Hardened Edition, msiexec.exe will attempt to make a connection to ocsp.digicert.com in order to validate the Acronis SCS binary signing certificate. 
 
Acronis Cyber Backup 12.5 SCS Hardened Edition (build 16731) contains binary wnaspi32.dll which is signed by AIG, not Acronis SCS. The CDRecord binary is located: C:\Program Files\Common Files\Acronis\CDRecord\wnaspi32.dll

Acronis Cyber Backup 12.5 SCS Hardened Edition (build 16731) utilizes third party drivers from the following companies:
 - Virtuozzo
 - LSI Logic
 - Microsoft
 - Realtek
 - Red Hat
 - VMware
 - Citrix Systems

*A further detailed list can be provided upon request
