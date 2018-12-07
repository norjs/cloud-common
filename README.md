Common files for NorJS's cloud framework
========================================

Install: `npm install --save '@norjs/cloud-common`

### `createBodyIDs()` -- Create unique identifier based on object content 

This function creates unique IDs for cloud objects based on their content.

```
import { createBodyIDs } from '@norjs/cloud-common';

let body = {
  hello: "world"
};
let id, hash;
[id, hash] = createBodyIDs(body);

body.$id = id;
body.$hash = hash;
```
