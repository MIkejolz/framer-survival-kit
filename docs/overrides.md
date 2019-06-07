## Overrides

Overrides allows you to override a field on the properties panel. One thing to take in consideration is that Overrides are just applied in the preview mode, not on the default Framer view.

The properties don't have to be static, Overrides support animation and interactions too, so it's a great way to animate elements that appear static on the normal view.

First you need to import Overrides:
```JavaScript
import { Override } from "framer"
```

Simple prop override:

```JavaScript
// Create a function that exports the prop override
export function BackgroundRed(): Override {
    return {
        background: "red"
    }
}
```

Overrides is useful for console log information as well, like when you want to find out object values by tap them. This is a example of a console log.

Console Log text on tap:

```JavaScript
export function LogTap(): Override {
    return {
        onTap: () => {
            console.log("Hello")
        },
    }
}
```


[Back to home page](../README.md)
