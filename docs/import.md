## Import Data

Import data from a json file is as easy as create the json, save inside the code folder, and add this import in the top of the page

Json file:
```json
{
    "user": {
        "name": "This is the name",
    		"details": {
                "email": "email@email.com"
            }
    }
}
```

Import user into the document:
```JavaScript
import { user } from "./data.json";
```

[Back to home page](../README.md)
