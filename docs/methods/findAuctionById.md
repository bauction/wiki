To find an auction by auction id.

return the Auction details.

## Usage

```js
findAuctionById(auction_id);
```

#### Parameters

> auction_id: String

## Example

```js
const auction_id = "80C4AB98-08B8-16D1-0000-000000000000";
const auction = await bauctionInstance.findAuctionById(auction_id); //returns auction details.
```
