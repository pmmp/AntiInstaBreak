## AntiInstaBreak
[![Poggit](https://poggit.pmmp.io/ci.shield/dktapps/AntiInstaBreak/AntiInstaBreak)](https://poggit.pmmp.io/ci/dktapps/AntiInstaBreak/AntiInstaBreak)

PocketMine-MP plugin implementing anti-cheat for instabreak.

### Background
This anti-cheat was originally built-in to the core. However, since it is unnecessary for vanilla gameplay, it has been removed from the core code.
This plugin was created in response to complaints received about its removal. 
As seen in the code, it is very easy to recreate within a plugin, further demonstrating the unnecessariness of it being in the core code at all.

### Caveats
This plugin is not guaranteed to be bug-free and suffers from all the same issues that the original built-in implementation did, such as:
- Haste and mining fatigue are not correctly accounted for, because their implementations differ in Minecraft Bedrock and nobody has successfully reproduced their behaviour externally. 
Many development hours were wasted on trying to get this right, so don't expect it to be fixed any time soon.
- Efficiency enchantment is not accounted for because it is not yet implemented into PocketMine-MP at the time of writing.
- Jumping, swimming and climbing ladders is not accounted for.
- Players may innocently trigger this anti-cheat if they hit a spot of network lag (more than 1 or 2 ticks).
