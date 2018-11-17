# EmpireEco
EmpireEco is an Item Based Economy plugin.
It was meant for RPG servers that wish to have a similar 
coin system like MMO games (e. g. WoW or GuildWars 2)

- Author: Benjamin83 (Tyler)
- Discord: T Y L E R#6343
- D-Server: https://discord.gg/3K6KQh3

# Syntaxes
# effects:

remove a specific amount of type of coins from player's vault. Behaves just like the command.
  - subtract %number% bronze|silver|gold (from|of) (%player%'s vault|vault of %player%)
   
add a specific amount of type of coins to player's vault. Behaves just like the command.
  - add %number% bronze|silver|gold to (%player%'s vault|vault of %player%)

Remove a specific amount of type of coins from player's inventory
  - remove %number% [of] bronze|silver|gold coin[s] from %player%'s inventory


# expressions:

If you want to get the amount of the player's type of coin.
  - %player%'s bronze|silver|gold

Get the amount of type of coin from player's inventory. Physical items.
  - [amount of] bronze|silver|gold [found] in %player%'s inventory

Get the yaml value of a module.
  - [empire[eco]] status (of|from) module %text%:


# conditions:

Condition to check if the module is true or false
  - [empire[eco]] status (of|from) module %text% is true|false:


# Support:
Support will only be given through discord, here or on Spigot.
