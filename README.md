# opportunityzones

## moving shelf notes

- Lower limit: 0
- Upper limit: 145,000

## to load program on controller
- Paste script into code space field
- click Compile
- click Download

## tell the controller to autorun the standalone script on boot

Paste the following commands in the "Terminal" field and press Enter/Return after each one

- `SLOAD=1` # Enter
- `STORE` # Enter

Unplug the controller, plug it back in, the script should auto run. If the controller is still connected to the computer via USB you will see the status of the program running (the current position and the line numbers of the script should be changing)
