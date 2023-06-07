Remove this from DogPathing.json in Always Raining if it causes issues. Tried moving "Season" into "When"

```jsonc
  //Thursday, Saturday
  {
    "LogName": "Max Path Sterling's Room",
    "Action": "EditMap",
    "Target": "Maps/Custom_ARVHouse",
    "MapTiles": [
      {
        "Position": {
          "X": "20",
          "Y": "22"
        },
        "Layer": "Back",
        "SetProperties": {
            "CustomCompanions": "Spawn 1 Himetarts.ARVCC.HenryDogPath"
        },
      },
    ],
    "When": { 
      "DayOfWeek": "Thursday, Saturday",
      "Weather":"Sun, Wind, Snow" 
    },
    "Season": "Spring, Fall, Winter",
    "Update": "OnLocationChange" 
  }, 
```