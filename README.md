# opportunityzones

## notes

```
Lower limit: 0
Upper limit: 145,000

"Download" refers to sending data _to_ the controller (a program script or settings)
"Upload" refers to retreiving data _from_ the controller (the already loaded program or settings)
```

Arcus motor controller:
[PMX-2ED-SA](https://www.arcus-technology.com/products/multi-axis-motion-controller/2-axis-usb-controller-plus-driver/)

Motors: [NEMA 17 stepper motor](https://www.arcus-technology.com/products/stepper-motors/nema-17/)

Docs are saved in this repo.

## save program to motor controller
- Connect the Arcus controller via USB
- Open the Arcus GUI program
- Connect to Arcus
- Paste the contents of our `arcus_shelf.prg` script into code space field
- click Compile
- click Download

## tell the controller to autorun the standalone program on boot

Paste the following commands in the "Terminal" field and press Enter/Return after each one

- `SLOAD=1` # Enter
- `STORE` # Enter

Unplug the controller, plug it back in, the script should auto run. If the controller is still connected to the computer via USB you will see the status of the program running (the current position and the line numbers of the script should be changing)


## unplugging the shelf

Do not unplug or power off the installation unless the motors are paused in the home position. The home position is marked on the motor rails.

If the installation looses power when the shelf is not in the home position it must be moved by hand. Physically push the shelf down to the marked home position, then plug the installation back in.
