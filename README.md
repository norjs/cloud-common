Common files for Sendanor's cloud framework
===========================================

Install: `npm install --save '@sendanor/cloud-common`

### `createBodyIDs()` -- Create unique identifier based on object content 

This function creates unique IDs for cloud objects based on their content.

```
import { createBodyIDs } from '@sendanor/cloud-common';

let body = {
  hello: "world"
};
let id, hash;
[id, hash] = createBodyIDs(body);

body.$id = id;
body.$hash = hash;
```
