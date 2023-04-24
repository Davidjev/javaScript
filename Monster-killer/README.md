# README file for project Monster-killer

This program is a simple game where a player battles a monster. The game involves two players: the player and the monster. The game has four attack modes: standard attack, strong attack, monster attack, and player heal. Each attack mode has a different effect on the game's variables.   

### Game variables

- ATTACK_VALUE: A constant variable with a value of 10. It is the default damage done by a standard attack.  
- STRONG_ATTACK_VALUE: A constant variable with a value of 17. It is the default damage done by a strong attack.  
- MONSTER_ATTACK_VALUE: A constant variable with a value of 14. It is the default damage done by a monster attack.  
- HEAL_VALUE: A constant variable with a value of 20. It is the default amount of health restored by a player heal.  
- MODE_ATTACK: A constant variable with a value of "ATTACK". It is used to represent the standard attack mode.  
- MODE_STRONG_ATTACK: A constant variable with a value of "STRONG_ATTACK". It is used to represent the strong attack mode.  
- LOG_EVENT_PLAYER_ATTACK: A constant variable with a value of "PLAYER_ATTACK". It is used to represent the event where the player makes a standard attack.  
- LOG_EVENT_PLAYER_STRONG_ATTACK: A constant variable with a value of "PLAYER_STRONG_ATTACK". It is used to represent the event where the player makes a strong attack.  
- LOG_EVENT_MONSTER_ATTACK: A constant variable with a value of "MONSTER_ATTACK". It is used to represent the event where the monster makes an attack.  
- LOG_EVENT_PLAYER_HEAL: A constant variable with a value of "PLAYER_HEAL". It is used to represent the event where the player heals.  
- LOG_EVENT_GAME_OVER: A constant variable with a value of "GAME_OVER". It is used to represent the event where the game ends.  
- battleLog: An array that stores all events that happen in the game. Each event is stored as an object with specific properties.  
- lastLoggedEntry: A variable used to track the last entry logged to the console.  
- chosenMaxLife: A variable that represents the maximum life value for the player and monster. It is set by the user via a prompt function.  
- currentMonsterHealth: A variable that represents the current health value for the monster. It is initialized to chosenMaxLife.  
- currentPlayerHealth: A variable that represents the current health value for the player. It is initialized to chosenMaxLife.  
- hasBonusLife: A boolean variable that determines if the player has an extra life.  

### Functions

- getMaxLifeValues(): A function that prompts the user to enter the maximum life value for the player and monster. If the user enters an invalid value, an error message is thrown. The function returns the parsed value.
- writeToLog(ev, val, monsterHealth, playerHealth): A function that writes an event log to the battleLog array. The function takes in four parameters: ev, val, monsterHealth, and playerHealth. The ev parameter specifies the event that occurred, the val parameter specifies the value associated with the event, monsterHealth specifies the monster's health value, and playerHealth specifies the player's health value.
- reset(): A function that resets the game variables to their initial values.
- endRound(): A function that represents a round in the game. It involves the monster attacking the player, the player potentially losing a bonus life, and the game ending if either the player or the monster's health drops to 0.
