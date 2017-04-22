# simple-raycaster

> 👆 Simple raycaster (cursor) for ReactVR

# Usage

In your `ReactVR`'s `client.js`:

```js
import { VRInstance } from "react-vr-web";
import * as SimpleRaycaster from "simple-raycaster";

function init(bundle, parent, options) {
  const vr = new VRInstance(bundle, "librarytests", parent, {
    raycasters: [
      SimpleRaycaster // Add SimpleRaycaster to the options
    ],
    cursorVisibility: "auto", // Add cursorVisibility
    ...options
  });
  vr.start();
  return vr;
}

window.ReactVR = { init };
```
# License

MIT. See [License](./LICENSE)
