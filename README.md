# opportunityzones

## notes

- Lower limit: 0
- Upper limit: 145,000

- "Download" refers to sending data _to_ the controller (a program script or settings)
- "Upload" refers to retreiving data _from_ the controller (the already loaded program or settings)

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
