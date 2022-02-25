# createProfile

Create profile for authenticated user.

Returns `true` on success, otherwise returns `Error`.

## Usage:

```js
updateMyProfile(name, location, about);
```

#### Parameters

> name: String

> location: String

> about: String

## Example

```js
const name = "user name";
const location = "united states";
const about = "about section";
const updated = await bauctionInstance.updateMyProfile(name, location, about); // returns true or Error.
```
