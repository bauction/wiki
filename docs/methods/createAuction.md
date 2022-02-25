# createAuction

To create any type of new auction.

Returns created auction.

## Usage

```js
createAuction(auctionInput);
```

#### Parameters

> auctionInput: Object, contains the fields to be updated.

> auctionInput = {
> name: Text;
> startDate: Text;
> endDate: Text;
> description: Text;
> minBidAmt: Nat;
> maxBidAmt: Nat;
> category: Text;
> location: Text;
> auctionType: AuctionDirectionType;
> }

> here, auctionDirectionType: enum ["ForwardAuction", "ReverseAuction", "ETender", "FlexibleOffers"]

> minBidAmt and maxBidAmt dependent upon type of auction. For Reverse Auction maxBidAmt will be considered and all bids will be less than maxBidAmt. For other type of auction minBidAmt will be considered minimum bid amount or base amount for that auction.

## Example

```js
const auctionInput = {
  name: "auction name",
  category: "digital art",
  startDate: "Mon Feb 07 2022 21:11:54",
  endDate: "Mon Feb 12 2022 21:11:54",
  description: "description of the auction",
  minBidAmt: 1000,
  category: "digital art",
  location: "location string",
  auctionType: "ForwardAuction",
};

const createdAuction = await bauctionInstance.createAuction(auctionInput); //returns created auction
```
