![image](https://github.com/mytechnotalent/MicroPython-micro-bit_How_To_Build_And_Freeze_Modules/blob/master/MPMBHTBAFM.png?raw=true)

# MicroPython micro:bit
# How To Build And Freeze Modules
This repo will teach you step-by-step how to build and freeze custom Python modules into the BBC micro:bit fork of MicroPython.  If you are an educator and want to develop custom modules you can include in the firmware this tutorial is for you.

#### This tutorial is based on Pye Douglas's work (@pyeprog).
#### [SOURCE: https://github.com/bbcmicrobit/micropython/issues/530#]

## STEP 1: Clone MicroPython for the BBC micro:bit Repo
```bash
git clone https://github.com/bbcmicrobit/micropython.git
```

## STEP 2: Copy LATEST make-frozen.py Module
#### SOURCE 
```bash
https://github.com/micropython/micropython/blob/master/tools/make-frozen.py
```
***PLACE FILE IN THE tools DIRECTORY AS make-frozen.py***

## STEP 3: Create frozen/firmware Directory
```bash
mkdir frozen
cd frozen
mkdir firmware
cd ..
```

## STEP 4: Create hello.py
```python
print('hello')
```
***PLACE FILE IN THE frozen/firmware DIRECTORY AS hello.py***

## STEP 5: Transform hello.py To hello.c
```bash
python tools/make-frozen.py <GIT_REPO_FOLDER_PATH>/frozen/firmware > hello.c
```

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
