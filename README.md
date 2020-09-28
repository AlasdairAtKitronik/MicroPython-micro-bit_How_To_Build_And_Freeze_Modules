![image](https://github.com/mytechnotalent/MicroPython-micro-bit_How_To_Build_And_Freeze_Modules/blob/master/MPMBHTBAFM.png?raw=true)

# MicroPython micro:bit
# How To Build And Freeze Modules
This repo will teach you step-by-step how to build and freeze custom Python modules into the BBC micro:bit fork of MicroPython.  If you are an educator and want to develop custom modules you can include in the firmware this tutorial is for you.

## STEP 5: Create main.py Module
#### SOURCE 
```python
while True:
    try:
        print('\n' * 100)
        print('Entry Point Loop')
        input('Press ENTER...')
    except KeyboardInterrupt:
        pass
```
***PLACE FILE IN THE SAME FOLDER AS _boot.py***

## STEP 6: Flash Firmware
#### Instructions 
```bash
https://github.com/micropython/micropython/tree/master/ports/esp32
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)
