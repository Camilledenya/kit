# Vanishers

Vanishers are objects that disappear and become uncollidable when touched.

## Use Cases

Vanishers can be used to create varying types of gameplay, puzzles, or contraptions.
An example of this is to speed up pacing for a section by requiring the player to move fast.

All Vanisher parts in the `VanisherGroup` model will be activated when any part in the model is touched.

## Vanish modes

Each `VanishMode` has unique logic.

| Mode |  Description
|:-----:|:-----:
| `Fade` | Smoothly fades.
| `Blink` | Flashes multiple times before vanishing.
| `Constant` | Gradually fades depending on contact. If not in contact, regenerates.
| `Shrink` | Shrinks the part away in a set direction (`Top`, `Bottom`, `Left`, `Right`, `Front`, `Back`, `Center`). Does not support trusses and may behave oddly with spheres.

## Configuration

| Name | Default Value | Description
|:-----:|:-----:|:-----:
| `BlinkCount` | 3 | Amount of blinks in `Blink` mode.
| `ConstantNoRecovery` | false | Prevents recovery in `Constant` mode when not in contact.
| `Invert` | false | Reverses behavior: visible becomes invisible and vice versa.
| `RespawnFade` | false | Whether the part fades in when respawning.
| `RespawnTime` | 2 | Seconds before the part reappears.
| `ShrinkDirection` | `Center` | [Direction of shrinking](#vanish-modes) in `Shrink` mode.
| `VanishMode` | `Fade` | [Vanish behavior](#vanish-modes).

If you add the `Invisible` tag to a `Vanisher` part, it will ignore all collision and transparency updates. This can be used for detail such as having one big selection box around a set of trusses.