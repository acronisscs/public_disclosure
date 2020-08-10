# Acronis SCS Cyber Backup 12.5 Hardened Edition Caveats

Acronis SCS Cyber Backup 12.5 Hardened Edition must be installed per the provided instructions in order to be fully DoDAPLin, Common Criteria, and FIPS compliant. The following items should be noted to ensure the desired functionality of the product:
 - RHEL6/Centos6 do not support keyring usage, therefore they are not supported in a fully compliant environment. 
 - CPUs must support RDRAND in order to be fully FIPS compliant. RDRAND provides an entropy source for the product and cannot achieve FIPS certification without it. 
 - Properly secured SSL certificates are required to be installed by the user, per the product user guide. 
 - Syslog must be utilized with the product and requires NXLog to be installed in order to forward appropriate logs. Installation and setup instructions are provided with the product user guide. 
