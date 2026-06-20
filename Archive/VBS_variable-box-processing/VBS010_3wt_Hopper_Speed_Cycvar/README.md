# 3wt Hopper Speed Cycvar
<img alt="simple_cycvar_v1_0_front.png" src="images/simple_cycvar_v1_0_front.png?raw=1" height="300px">

**Authors:** *iigo*

**Endorsed by:** *TisUnfortunate*

**Tags:** *Functional*

**Original post:** [View on Discord](https://discord.com/channels/1375556143186837695/1517738568137576499)

A compact (3x7x12 slice) hopper speed cyclical variable sorter that splits and merges a batch of mixed boxes while producing minimal partial boxes. Ready to use with a cubic footprint.
## Features
- 3x7x12 slice dimensions
- 54 box batch size
- Handles empty boxes, 64 unstackables, 16 unstackables, and unstackable items
- Can pause to stop new cycles from starting
- Will not start a cycle without sufficient empty boxes
- isActive readout
- Empty boxes early exit when entering unset slice
- Empty box check integrated with end slice
- Ideal output (minimal partial boxes)
- Fully hopper unlocked
- Nether compatible
- 29 box buffer between slices
## Considerations
- Empty boxes and unstackable items share a output chest
- Only input at most 54 boxes in each batch; use the isActive readout for batching inputs
- Pause may take some time to occur since it will finish current cycle; use isActive to determine when safe to unload
- If using pause, take input batching into account since buffer will still have items in it but isActive will read false
- Only input boxes into the input or equivalent hopper line
- No overflow protection on output chests; ensure that they do not back up into slices to prevent errors and item loss
- Item count in hopper clock is dependent on number of slices
## Instructions
1. Use the isActive readout for batching inputs (input at most 54 boxes in each batch).
2. If pausing, use isActive to determine when it is safe to unload (pause finishes the current cycle).
3. Avoid output chest back-ups into slices to prevent errors and item loss.
4. Only input boxes into the input or equivalent hopper line.

## Resources
- [VBS010_simple_cycvar_v1_0_iigo.litematic](attachments/VBS010_simple_cycvar_v1_0_iigo.litematic): MC 1.21.11, Size 7x12x35 blocks
