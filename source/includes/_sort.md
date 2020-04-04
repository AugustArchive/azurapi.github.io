# Sorting Information
> The functions below returns JSON structured like this:

```json
{
  /* same as getting ships in array */
}
```

This Section contains all the ships being sorted in an array according to the relevant functions indicated by the developers.

## Sorting Ships
### Sort ships by ID
```javascript
const azurlane = require('@azurapi/azurapi')
azurlane.getAllShipsById()
//or
import { getAllShipsById  } from '@azurapi/azurapi'
console.log(getAllShipsById())
```

### Sort ships by Names in different languages
```javascript
import { getAllShipsByEnglishName  } from '@azurapi/azurapi' //ES6
//const { getAllShipsByEnglishName  } = require('@azurapi/azurapi') ES5
console.log(getAllShipsByEnglishName())
```

| Languages | JS                        |
|-----------|---------------------------|
| Unfiltered| getAllShips               |
| English   | getAllShipsByEnglishName  |
| Japanese  | getAllShipsByJapaneseName |
| Chinese   | getAllShipsByChineseName  |
| Korean    | getAllShipsByKoreanName   |

### Filter ships by Faction/Nationality
```javascript
const azurlane = require('@azurapi/azurapi')
azurlane.getAllShipsFromNation();
azurlane.getAllShipsFromNationality();
azurlane.getAllShipsFromFaction();
//or
import { getAllShipsFromNation, getAllShipsFromNationality, getAllShipsFromFaction } from '@azurapi/azurapi'
console.log(getAllShipsFromNation())
console.log(getAllShipsFromNationality())
console.log(getAllShipsFromFaction())
```
## Sorting Equipment

###Sort Equipment by Name
```javascript
import { getAllEquipments  } from '@azurapi/azurapi' //ES6
//const { getAllEquipments  } = require('@azurapi/azurapi') ES5
console.log(getAllEquipments())
```

| Languages | JS                        |
|-----------|---------------------------|
| Unfiltered| getAllEquipments          |
| Official  | getEquipmentByOfficialName|