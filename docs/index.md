## Overview

Bauction is a **decentralized, distributed, peer-to-peer auction platform**.

Bauction uses [Internet Computer Protocol](https://dfinity.org/) as platform to host and store auction data over blockchain. Bauction is one of the first platform to provide fully decentralized platform for auctioning rare items over the decentralized web.

## **Installation:**

```
yarn add bauction-js
```

or

```
npm install bauction-js
```

## **Basic Usage**

```js
import Bauction from "bauction-js";
const bauctionInstance = new Bauction();
//use async function for this:
await bauctionInstance.initIdentity("path-to-secret-key");

bauctionInstance.getAllAuctions(); //to fetch all auctions from bauction canister.
```

## **Example**

```js
import Bauction from "bauction-js";
const bauctionIns = new Bauction();

const initializeBauction = async () => {
  await bauctionIns.initIdentity("/root/user/my_secret_key.cer");
};

initializeBauction();

bauctionIns.getMyAuctions(); //returns all auctions created by identity bauction is initialized with.
```
