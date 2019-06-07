## Create and modify controls

Controls is a great way to define what you want to be editable in a frame(object).

Resources:
```JavaScript
// https://www.framer.com/api/property-controls/
```

Import controls:
```JavaScript
import * as React from "react"
import { Frame, addPropertyControls, ControlType } from "framer"
```


Add a controls:
```JavaScript
// Add property control to the properties panel
addPropertyControls(Control_code_comp, {
    text: {
        type: ControlType.String,
        title: "Text"
    },
})
```


Define default values:
```JavaScript
// Define the default value
Control_code_comp.defaultProps = {
    text: "Hello World!!!!",
}
```


Export frame:
```JavaScript
// Export frame
export function Control_code_comp(props) {
    return <Frame>{props.text}</Frame>
}
```


Full example:
```JavaScript
import * as React from "react"
import { Frame, addPropertyControls, ControlType } from "framer"

// best resources: https://www.framer.com/api/property-controls/

// Add property control to the properties panel
addPropertyControls(Control_code_comp, {
    text: {
        type: ControlType.String,
        title: "Text"
    },
})

// Define the default value
Control_code_comp.defaultProps = {
    text: "Hello World!!!!",
}

// Export frame
export function Control_code_comp(props) {
    return <Frame>{props.text}</Frame>
}
```

[Back to home page](../README.md)
