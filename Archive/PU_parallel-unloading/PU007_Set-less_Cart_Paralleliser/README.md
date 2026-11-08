# Set-less Cart Paralleliser
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *Andrews54757, TisUnfortunate, javierrubik33*

**Endorsed by:** *TPS Nighthunter*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1569105915116781739)

A device that can release up to 16 items in parallel at hopper speed each, allowing for faster sorting in a filter-based storage system.
## Features
- Up to 16× hopper-speed sorting (141,750 items/hour)
- Accepts any item as input
- Outputs unstackable items
- Cheap and small: 8×8×7
- Few inventories to fill
- Entity read-out can register up to 150 entities
- Refresh carts reset the despawn timer for items each cycle and can be configured to accept approximately 300 entities
## Considerations
- Directional; should not be rotated or mirrored
- Stacks release with a size up to 63, so only low-threshold item filters may be used
- Uses a high count of entities, which are almost always still
- There is no way to limit the user. A player can throw large amounts of items by hand; exceeding the entity-count limit may cause despawns. A box unloader is recommended.
- Items are not sorted at exactly hopper speed; 8 game ticks of extra delay were added between cycles to account for more types of filters.
## Notes
Logic designed by Andrews54757. Wiring and logic optimisation by TisUnfortunate.

## Resources
- [PU007_Cart_Paralleliser_Javi.litematic](attachments/PU007_Cart_Paralleliser_Javi.litematic): MC 26.3, Size 8x8x7 blocks
