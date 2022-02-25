# updateAuction

To update an auction.

## **Note**

1. Only auction which are not started yet, can be updated.
2. Only auction creator can update the auction.
3. Only name, description and category can updated.

On success, returns updated auction.

## Usage

```js
updateAuction(auction_id, auctionUpdates);
```

#### Parameters

> auction_id: String

> auctionUpdates: Object, contains the fields to be updated.

> auctionUpdates = {
> name: String,
> description: String,
> category: String
> }

## Example

```js
const auction_id = "80C4AB98-08B8-16D1-0000-000000000000";

const auctionUpdates = {
  name: "updated name",
  description: "updated auction description",
  category: "digital art",
};

const updatedAuction = await bauctionInstance.updateAuction(
  auction_id,
  auctionUpdates
); //returns updated auction
```
