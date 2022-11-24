# Cherry Market Subgraph

[Cherry Market](#) is a decentralized protocol for nft markerpalce.

This subgraph dynamically tracks any nft listed by the Cherry Market protocol.

- aggregated data about active items
- data about Item Bought
- data about ItemCanceled
- data about ItemListed

## Example Queries

### Querying Aggregated Active Items

This query fetches aggredated data from all item has been listed.

```graphql
{
        activeItems(first: 15, where: { buyer: "0x000000000000000000000000000000000000dead" }) {
            id
            buyer
            seller
            nftAddress
            tokenId
            prcie}
}
```
