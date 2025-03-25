# FiveMVehicle Documentation

## Overview
The `FiveMVehicle` class provides an interface to interact with a vehicle in FiveM.

## Methods

### `get rpm()`
- **Returns**: The current RPM of the vehicle.
- **See**: [GetVehicleCurrentRpm](https://docs.fivem.net/natives/?_0xE7B12B54)

### `set rpm(rpm: number)`
- **Parameter**: `rpm` - The desired RPM to set.
- **See**: [SetVehicleCurrentRpm](https://docs.fivem.net/natives/?_0x2A01A8FC)

### `get speed()`
- **Returns**: The current speed of the vehicle in km/h.
- **See**: [GetEntitySpeed](https://docs.fivem.net/natives/?_0xD5037BA82E12416F)

### `set engineOn(state: boolean)`
- **Parameter**: `state` - A boolean indicating whether to turn the engine on (true) or off (false).
- **See**: [SetVehicleEngineOn](https://docs.fivem.net/natives/?_0x2497C4717C8B881E)

### `get lockstate()`
- **Returns**: The lock state of the vehicle, corresponding to a value from the `eVehicleLockState` enum.
- **See**: [GetVehicleDoorLockStatus](https://docs.fivem.net/natives/?_0x25BC98A59C2EA962)

### `set lockstate(state: number)`
- **Parameter**: `state` - The lock state, corresponding to a value from the `eVehicleLockState` enum.
- **See**: [SetVehicleDoorsLocked](https://docs.fivem.net/natives/?_0xB664292EAECF7FA6)

# FiveMPlayer Documentation

## Overview
The `FiveMPlayer` class provides an interface to interact with a player in FiveM.

## Methods

### `get position(): Vector3`
- **Returns**: The position of the player as a {@link Vector3}.
- **See**: [GetEntityCoords](https://docs.fivem.net/natives/?_0x3FEF770D40960D5A) / {@link TransformNumberArrayInVector3} for more information.

### `set position(newPosition: Vector3 | [number, number, number])`
- **Parameter**: `newPosition` - The position as a {@link Vector3} or a NumberArray.
- **See**: [SetEntityCoords](https://docs.fivem.net/natives/?_0xDF70B41B) for more information.

### `get collision(): boolean`
- **Returns**: `true` if the player's collision is enabled; `false` if it is disabled.
- **See**: [GetEntityCollisionDisabled](https://docs.fivem.net/natives/?_0xCCF1E97BEFDAE480) for more information.

### `set collision(enable: boolean)`
- **Parameter**: `enable` - `true` to enable collision, `false` to disable it.
- **See**: [SetEntityCollision](https://docs.fivem.net/natives/?_0x1A9205C1B9EE827F) for more information.

### `get frozen(): boolean`
- **Returns**: `true` if the player is frozen; `false` if not.
- **See**: [IsEntityPositionFrozen](https://docs.fivem.net/natives/?_0xEDBE6ADD) for more information.

### `set frozen(enable: boolean)`
- **Parameter**: `enable` - `true` to freeze the player, `false` to unfreeze.
- **See**: [FreezeEntityPosition](https://docs.fivem.net/natives/?_0x65C16D57) for more information.

## Usage Example

```typescript
const player = new FiveMPlayer(GetPlayerPedId();
const vehicle = new FiveMVehicle(GetVehiclePedIsIn(PlayerPedId(), false););
````
