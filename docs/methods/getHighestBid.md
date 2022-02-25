# getHighestBid

Returns the highest bid of the auction.

On success, return the highest bid of the auction.

## **Note**

1. In case of E-Tenders, highest bid will always return 0, as bid are not exposed till the auction gets over.
2. Highest bid is subjective to the type of auction. In case of Reverse auction, most minimum bid will be returned, In case of flexible offers and Forward auctions, maximum bid will be returned.

## Usage

```js
getHighestBid(auction_id);
```

#### Parameters

> auction_id: String

## Example

```js
const auction_id = "80C4AB98-08B8-16D1-0000-000000000000";
const highestBid = await bauctionInstance.getHighestBid(auction_id); //returns highest bid (Natural number)
```
