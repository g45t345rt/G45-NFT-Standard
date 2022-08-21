# G45-ATC Standard

`DO NOT USE - STILL UNDER REVIEW`

This is just a smart contract to list your assets in a decentalized way.  
You can pair this with G45-AT to create an NFT collection.  

## Functions

### SetAsset

Set an asset to the collection. Increment `assetCount` if does not already exists.

- asset = SCID of the asset smart contract
- index = whatever index/number representing the asset

### DelAsset

Remove asset from collection

- asset = SCID of the asset smart contract

### Freeze

Freeze metadata or collection. Make variables immutable.  

- collection = 0:skip, 1:freeze
- metadata = 0:skip, 1:freeze

### SetMetadata

Change collection metadata if not frozen

- format = declare metadata format (usually json)
- metadata = Check InitStore metadata example

### TransferOwnership

Initiate new smart contract ownership

- newOwner = wallet address

### CancelOwnership

Cancel pending ownership transfer

### ClaimOwnership

Claim pending ownership