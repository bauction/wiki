To bid on any type of auction.

On success, returns true otherwise false.

## Usage

```js
bidOnAuction(auction_id, bidAmmount);
```

#### Parameters

> auction_id: String

> bidAmount: Natural number

## Example

```js
const auction_id = "80C4AB98-08B8-16D1-0000-000000000000";
const bidAdded = await bauctionInstance.bidOnAuction(auction_id, 8000); //returns true or false
```
