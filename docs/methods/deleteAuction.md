# deleteAuction

To delete an auction.

## **Note**

1. Only auction which haven't started yet, can be deleted.
2. Only auction creator is allowed to delete the auction.

On success, returns true, otherwise returns Error.

## Usage

```js
deleteAuction(auction_id);
```

#### Parameters

> auction_id: String

## Example

```js
const auction_id = "80C4AB98-08B8-16D1-0000-000000000000";
const deleted = await bauctionInstance.bidOnAuction(auction_id); //returns true or Error
```
