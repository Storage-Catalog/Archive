# Tis a Cart Splitter
<img alt="image.png" src="images/image.png?raw=1" height="300px">

**Authors:** *TisUnfortunate*

**Endorsed by:** *Ragdoll Willy*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1570939080596787330)

A device with item handling, cart loading, and box input/output features.
## Features
- 11 x 14 x 4wt
- 0gt between carts; items within an item type are pulled at 8x HS
- Splits HermitCraft8 items at 6.3x HS (57000 I/H)
- Random input proof
- Water stream empty box input
- Water stream unstackable and split box output
- 26 hoppers (2 locked)
- No idle carts
- Empty box proof
## Considerations
- Empty box collection will lose about 1/1500 boxes
- Buffers an empty box
## Notes
Slice locks for a duration after all boxes are processed to allow the idless-cart loader to power down; it remains unlocked until all boxes are cleared. The threshold for the next cart to check for the same type is 19. The first cart of each type pulls 27; every cart after pulls 28. There are 10–38 gt between item types, depending on final stack size.

## Resources
- [VIP013_Tis.A.Cart.Splitterv3.521.litematic](attachments/VIP013_Tis.A.Cart.Splitterv3.521.litematic): MC 1.21.4, Size 11x15x7 blocks
