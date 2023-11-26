![Piscine game](https://private-user-images.githubusercontent.com/89268663/262896853-03a6d09a-905b-44c0-99ae-54fdb13b9295.gif?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE3MDA5NzU4MTQsIm5iZiI6MTcwMDk3NTUxNCwicGF0aCI6Ii84OTI2ODY2My8yNjI4OTY4NTMtMDNhNmQwOWEtOTA1Yi00NGMwLTk5YWUtNTRmZGIxM2I5Mjk1LmdpZj9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFJV05KWUFYNENTVkVINTNBJTJGMjAyMzExMjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMxMTI2VDA1MTE1NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVlYmNjMjEwMzhlNDUwOWE1ZGU5ZDVjOWNhM2Y5ZjJkMWUzMjc4NTY1NzU4ZDZhMTQ3MWEwZmZlMjliMWFhYjQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Lmwrl5JdpccQX14RmR-nCuJ6iLFYuBhxaYvkjZaB2ZE)

The so_long is a game. In this Project your goal is to use a very simple and basic library, but very intuitive, the Minilibx.

My project was written in C using the concept of objects. Everything on display is an Object, from the floor and the walls, to the Player itself.

The game is themed around the 42 Piscine. The goal of the game, as a Pisciner, is to Collect 'Memory Addresses', avoid 'Seg Faults' and finally get to the 'Exit Pointer'. To achieve your goal you are able to control and move the 'Seg Faults'.

To achieve Movement and Collision, the floor was used as a Bidimensional HashTable. If an Object is not a piece of floor or a piece o wall, it will then be on_top of another object. The Floor objects have a linked list to all the objects standing in its area. When an Object moves, it will check the floor's around it, and verify if they have in their linked list another object "on top" of them. If there is, their distance is calculated to verify if they are colliding, and if they are, what actions have to be taken.

Instructions: 

  - Start Game: To start the game you have to open the so_long Folder in a Linux Terminal, and type the command "./so_long" followed by the name of the map file finished by ".ber". Ex: "./so_long map.ber" ou "./so_long 2map.ber"
  - Goal: Your goal is to Collect 'Memory Addresses', avoid 'Seg Faults' and finally get to the 'Exit Pointer'. If a 'Seg Fault' touches the Player or a 'Memory Address'
you fail.
  - Movement: | WASD |.
  - Ability.Move_Fire: | Space |. You are able to move all 'Seg Faults' at the same time, they will move in the same direction and at the same time that the player does.
One tap will activate movement, another tap will deactivate. Avoid holding Space since it will switch it on and off continuously.


