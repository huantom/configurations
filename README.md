# configurations
Synchronizers, Validators and Custodians could submit issues to configure their public parameters, e.g. name, logo, descriptions.
exSat Foundation will check with the issues and submit pull request to integrate it.

# Synchronizers
There are two types of information that need to be configured for a Synchronizer:

- **Synchronizer Registration Information**: If the mining pool needs to register as a Synchronizer before exSat catches up with the latest BTC blocks, you should add the "mining_addresses" field in the configuration, which contains all the mining addresses of the mining pool. Please note that this information is public on GitHub, and anyone who accesses the current GitHub repository can see it.

- **Synchronizer Identity Information**: Such as name, icon, website, and introduction. Please note that this information is public on the front-end page, and anyone who accesses the Synchronizer front-end page can see it.

Here's an example from a fabricated mining pool:
```json
{
    "name": "CoolPool",
    "synchronizer": "coolpool.sat",
    "miningAddress": ["tb1qn6f3ngc9a426dzu9qw569yu9vj9ntjza4zjqz3",
                      "tb1qn6f3ngc9a426dzu9qw569yu9vj9ntjza4zjqz2"],
    "link": "https://coolpool.com",
    "logoURI": "https://cool.network/img/logo.png",
    "introduction": "A cool pool."
  }
```

# Validators
Validators can configure its information in this way, the informations can be seen by everyone on the front-end interface. 
Here's an example from a fabricated validator:
```json
{
    "name": "TrustGP",
    "validator": "trustgp.sat",
    "link": "https://trustgp.com",
    "logoURI": "https://trustgp.network/img/logo.png",
    "introduction": "TrustGP is a asset group."
  }
```

