# BattleShip Program
## By Bruce Garcia, Jashua Lioy, Chase McWhirt, Tsewei Peng

Link to [Java Code](https://github.com/OSU-CS361-W17/group8_project1/tree/master/src/main/java/edu/oregonstate/cs361/battleship)

Link to [Front-End Code](https://github.com/OSU-CS361-W17/group8_project1/tree/master/src/main/resources/public)

### Current Data Structure:
```json
{
    "aircraftCarrier": {
        "name": "AircraftCarrier",
        "length": 5,  
        "start": { "row": 0,"col": 0 },
        "end": {"row": 0, "col": 0}
    },
    ... 
    "computer_aircraftCarrier": {
        "name": "Computer_AircraftCarrier",
        "length": 5,
        "start": { "Across": 2,"Down": 2 },
        "end": {"Across": 2, "Down": 7}
    },
    "computer_battleship": {
        "name": "Computer_Battleship",
        "length": 4,
        "start": { "Across": 2,"Down": 8 },
        "end": {"Across": 6, "Down": 8}
    },
    "computer_cruiser": {
        "name": "Computer_Cruiser",
        "length": 3,
        "start": { "Across": 4, "Down": 1 },
        "end": {"Across": 4, "Down": 4}
    },
    "computer_destroyer": {
        "name": "Computer_Destroyer",
        "length": 2,
        "start": { "Across": 7, "Down": 3 },
        "end": {"Across": 7, "Down": 5}
    },
    "computer_submarine": {
        "name": "Computer_Submarine",
        "length": 2,
        "start": { "Across": 9, "Down": 6 },
        "end": {"Across": 9, "Down": 8}
    },
    "playerHits": [{row: 5, col: 10}...],
    "playerMisses": [{row: 4, col: 10}...],
    "computerHits": [{row: 2, col, 1}...],
    "computerMisses": [row: 10, col: 5}...]
}
```
### To start battleship:
Type this in brower:
```
localhost:4567
```
### Placing ship request:
```
http://localhost:4567/placeShip/{shipname}/{across}/{down}/{horizontal | vertical}
```
an example request is:
```
http://localhost:4567/placeShip/aircraftCarrier/1/1/horizontal
```

### User fire request:
```
http://localhost:4567/fire/{across}/{down}
```
an example request is:
```
http://localhost:4567/fire/4/3
```