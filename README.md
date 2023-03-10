# Blacklist-for-Proton

Any BP from Proton blockchain is welcome to use our blacklist.

Config Options for eosio::chain_plugin:

```
  --actor-whitelist arg                 Account added to actor whitelist (may 
                                        specify multiple times)
  
  --actor-blacklist arg                 Account added to actor blacklist (may 
                                        specify multiple times)
  
  --contract-whitelist arg              Contract account added to contract 
                                        whitelist (may specify multiple times)
  
  --contract-blacklist arg              Contract account added to contract 
                                        blacklist (may specify multiple times)
  
  --action-blacklist arg                Action (in the form code::action) added
                                        to action blacklist (may specify 
                                        multiple times)
```

Run this script to download and add to the end of file config.ini

Check integraty of the file (```4e8a2e3daf14af1327994f8d38bbcd8e09574b844229f4f78c7bb96fd2560c26```):

```
sha256sum blacklist.ini
```

```
#!/bin/bash

# Download the blacklist.ini file
curl -O https://raw.githubusercontent.com/alvosec/Blacklist-for-Proton/main/blacklist.ini

cat blacklist.ini >> /opt/ProtonMainNet/protonNode/config.ini
```
