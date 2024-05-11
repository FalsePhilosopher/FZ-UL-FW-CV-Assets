# FZ-UL-FW-CV-Assets
Asset swap for Unleashed firmware inspired by a 90's portable cartridge game console rom hack of "battle monsters" red.<br>
https://archive.org/download/PokemonCockVersion/Pokemon%20-%20Cock%20Version%20%28Bootleg%29.zip <br>
size=375378 (366.6 KiB)<br>
md5=6ad910a77b3c6a753a46af51a8efefd2<br>
crc32=480b1bf4<br>
sha1=218dedd4f38e25fc871053e5bdbbc9bfe5d7957a

# Instructions to build/maintain your own CV FW
1. `git clone https://github.com/FalsePhilosopher/CE-FW-assets`<br>
2. For OFW `git clone --recursive https://github.com/flipperdevices/flipperzero-firmware`<br> for UL `git clone --recursive https://github.com/DarkFlippers/unleashed-firmware.git`<br>
3. Overwrite the dolphin meta assets located `FW root folder>assets>dolphin` using the ones provided in this repo.<br>
4. Build the FW(refer to fbt.md  for more info on how [here](https://github.com/flipperdevices/flipperzero-firmware/blob/dev/documentation/fbt.md)) `./fbt COMPACT=1 DEBUG=0 updater_package`
5. For updates
- go to FW folder and pull updates `git pull`<br>
- clear build files `./fbt COMPACT=1 DEBUG=0 updater_package -c`<br>
- build fw `./fbt COMPACT=1 DEBUG=0 updater_package`
