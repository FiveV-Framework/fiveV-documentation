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

## Lock State Enum
- `0`: VEHICLELOCK_NONE
- `1`: VEHICLELOCK_UNLOCKED
- `2`: VEHICLELOCK_LOCKED
- `3`: VEHICLELOCK_LOCKOUT_PLAYER_ONLY
- `4`: VEHICLELOCK_LOCKED_PLAYER_INSIDE
- `5`: VEHICLELOCK_LOCKED_INITIALLY
- `6`: VEHICLELOCK_FORCE_SHUT_DOORS
- `7`: VEHICLELOCK_LOCKED_BUT_CAN_BE_DAMAGED
- `8`: VEHICLELOCK_LOCKED_BUT_BOOT_UNLOCKED
- `9`: VEHICLELOCK_LOCKED_NO_PASSENGERS
- `10`: VEHICLELOCK_CANNOT_ENTER
