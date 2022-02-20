
## Acceleration
Under the `[printer]` section there is some commented out acceleration settings that should be used for the first moves. You should comment out the existing setting for: 
`max_velocity`
`max_accel`
`max_z_velocity`
`max_z_accel`

And uncomment the section starting with:
`## Safe acceleration settings`
`## Use these for your first moves and sanity checks.`

## Z-Offset

This config contains a pre-saved z-offset for the probe, you **must** run a probe_calibrate before attempting to print to determine your own offset. Damage to the build surface might occur if you do not do this.

For example in klipper you will need to run:
`PROBE_CALIBRATE`

See https://github.com/Klipper3d/klipper/blob/master/docs/Probe_Calibrate.md for more details.