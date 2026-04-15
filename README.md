# Single-Player Version Modifications

This documentation outlines the changes made to the Nepali City Game to convert it from a multiplayer to a single-player version. Key files have been modified to remove all multiplayer networking functionalities.

## Modifications Applied

1. **player_character.gd**: Adjusted to remove ENet references and make character control local-only.
2. **vehicle.gd**: Modified to ensure vehicles operate without networked syncing.
3. **game.gd**: Updated to handle game logic for single-player without relying on multiplayer hooks.

### Key Changes in each file
#### player_character.gd
- Removed ENet connection setup and handling logic.
- Adjusted player movement to be fully local.

#### vehicle.gd
- Deleted multiplayer vehicle communication logic.
- Ensured all vehicle interactions are local.

#### game.gd
- Reconfigured game state management to eliminate reliance on multiplayer events.


## Future Improvements

Consider adding features to enhance single-player experience, such as AI competitors or additional gameplay modes.