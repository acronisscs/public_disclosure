# Acronis SCS Cyber Backup 12.5 Hardened Edition Caveats

Acronis SCS Cyber Backup 12.5 Hardened Edition must be installed per the provided instructions in order to run in fully DoDin APL, Common Criteria, and FIPS 140-2 compliant opertation. The following items should be noted to ensure the desired functionality of the product with regards to a certified environment:
 - RHEL6/Centos6 do not support OS keyring usage, therefore master secrets only have file protections instead of OS keyring protections. 
 - CPUs must support RDRAND in order to be fully FIPS 140-2 compliant. RDRAND provides a high quality documented entropy source for the product. 
 - Properly issued and signed x509 SSL certificates are required to be installed by the user, per the product user guide. 
 - Syslog must be utilized with the product and per our guidance, NXLog can be installed in order to forward appropriate logs. Installation and setup instructions are provided with the product user guide and KB.
