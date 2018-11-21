# EmpireEco
EmpireEco is an Item Based Economy plugin.
It was meant for RPG servers that wish to have a similar 
coin system like MMO games (e. g. WoW or GuildWars 2)

- Author: Benjamin83 (Tyler)
- Discord: T Y L E R#6343
- D-Server: https://discord.gg/3K6KQh3

## Syntaxes

### effect (subtract coins)

#### Syntax

`[empire[eco]] subtract %number% bronze|silver|gold (from|of) (%player%'s vault|vault of %player%)`

### Example

```
#remove a specific amount of type of coins from player's vault. Behaves just like the command.
subtract 5 gold from player's vault
```

---

### effect (add coins)

#### Syntax

`[empire[eco]] add %number% bronze|silver|gold to (%player%'s vault|vault of %player%)`

#### Example

```
#add a specific amount of type of coins to player's vault. Behaves just like the command.
add 5 gold to player's vault
```

---

### effect (remove coin from inventory)

#### Syntax

`[empire[eco]] remove %number% [of] [(1¦bronze)] [(2¦silver)] [(3¦gold)] coin[s] from [the] %player%'s inventory`

#### Example

```
#Remove a specific amount of type of coins from player's inventory
remove 5 gold coins from player's inventory
```

---

### expression (player's coins)

#### Syntax

`%player%'s bronze|silver|gold`

#### Example

```
#If you want to get the amount of the player's type of coin.
set {_test} to player's gold
broadcast "%{_test}%"
```
or
```
broadcast "%player's gold%"
``` 

---

### expression (coins in inventory)

#### Syntax

`[amount of] bronze|silver|gold [found] in %player%'s inventory`

#### Example

```
#Get the amount of type of coin from player's inventory. Physical items.
if gold found in player's inventory >= 40:
  remove 40 gold coins from player's inventory
  give player 1 apple named "&aGod Apple"
```
