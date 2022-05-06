## **Installation**

```
yarn add @bauction/sdk-js
```

or

```
npm install @bauction/sdk-js
```

## **Basic Usage**

```javascript
import Bauction from "@bauction/sdk-js";
const bauctionInstance = new Bauction();
//use async function for this:
await bauctionInstance.initIdentity("path-to-secret-key");

bauctionInstance.getAllAuctions(); //to fetch all auctions from bauction canister.
```

## **Example**

```js
import Bauction from "@bauction/sdk-js";
const bauctionIns = new Bauction();

const initializeBauction = async () => {
  await bauctionIns.initIdentity("/root/user/my_secret_key.cer");
};

initializeBauction();

bauctionIns.getMyAuctions(); //returns all auctions created by identity bauction is initialized with.
```
