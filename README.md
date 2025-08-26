# EKS Cell Door Control

Lightweight, configurable cell door system for custody vehicles using `ox_lib` and `ox_target`.

## Features

* Third-eye interaction at the rear of configured vehicles
* Open / Close cell doors (per-vehicle door indexes)
* Lock / Unlock cell doors
* Plays sound effect on lock and unlock
* Clean notifications via `ox_lib`

## Installation

1. Drag and drop the folder into your `resources/` directory

2. Add the following to your `server.cfg`:

   ensure EKS_PTV

3. (Optional) Edit `config.lua` to customize.

## Configuration

Define which doors count as �cell doors� for each vehicle model.

Door indexes:
`0 = Front Left`, `1 = Front Right`, `2 = Rear Left`, `3 = Rear Right`, `5 = Trunk`


Config.CellVehicles = {
    ['policet'] = {2, 3},   -- rear left + rear right
    ['riot']    = {5},      -- trunk as cage door
    ['police2'] = {2, 3, 5} -- rear + trunk
}


## Support

For help or customization, open a ticket through EKS.

https://discord.gg/busQ9w6dqa
