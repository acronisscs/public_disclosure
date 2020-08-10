# Acronis SCS Cyber Backup 12.5 Hardened Edition Caveats

Acronis SCS Cyber Backup 12.5 Hardened Edition must be installed per the provided instructions. The following items should be noted to ensure the desired functionality of the product:
 - No secure storage for RHEL6/Centos6
 - No FIPS for CPUs that don't support RDRAND
 - Proper SSL certificates are required to be installed by the user
 - NXLog required by the user for systems that need syslog support
