# Blacklist-for-Proton
Blacklist for Proton blockchain

Any BP from Proton blockchain is welcome to use our blacklist.

Run this script to download and add to the end of file config.ini

#!/bin/bash

# Download the blacklist.ini file
curl -O https://raw.githubusercontent.com/alvosec/Blacklist-for-Proton/main/blacklist.ini

cat blacklist.ini >> config.ini
