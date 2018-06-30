# ATD-Tokens

Payments & Budget Management Decentralized App
 
Leveraging the Blockchain, Cryptocurrency and AI Technologies

# Creating a Token:

Creating Standard tokens on EOS has following steps:
1. Create a new account on which tokens contract is to be deployed, using either <a href="https://toolkit.genereos.io/create">genereos toolkit</a> genereos toolkit or cleos:
cleos -u http://nodeosHost:port system newaccount Creator_name NewAccount_name owner_public_key active_public_key --stake-net "1 EOS" --stake-cpu "1 EOS" --buy-ram-kbytes "250 kiB" -p creator_name
2. Now, deploy the eosio.token contract using cleos:
cleos -u http://nodeosHost:port set contract account contract-dir [wast-file] [abi-file] -p account
3. Create new tokens using cleos:
cleos -u http://nodeosHost:port push action NewAccount_name create '{"issuer":"NewAccount_name", "maximum_supply":"15000000000.0000 ATD"}' -p  NewAccount_name
4. Issue Tokens to any account:
 cleos -u http://nodeosHost:port push action NewAccount_name issue '[ "receiver", "100.0000 ATD", "memo" ]' -p NewAccount_name

Congratulations, you’ve created your own standard tokens on EOS!

**ATD tokens have been created in the same way

Please reach us at:

<a href="http://t.me/atidium">Telegram</a>

<a href="https://www.atidium.io/">Atidium.io</a>

<a href="https://www.linkedin.com/company/atidium/">Linkedin</a>

<a href="https://www.youtube.com/channel/UCEsqXclpqLji2sG3X7ezHeg">Youtube</a>

<a href="https://www.reddit.com/user/atidium-network">Reddit</a>
