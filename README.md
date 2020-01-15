![image](davan.png 'da van')

# board_configs

The following are config files for my mechanical keybaords.

Config files can be generated [here](https://qmk.thevankeyboards.com/).

## keyboards

- [Work Keyboard](work_van/WORKVAN.md) - Minivan Kumo
- [Home/Travel Keyboard](travel_van/TRAVELVAN.md) - Minivan Atom

## Libraries needed to flash boards

```
brew install dfu-programmer
```

## Steps to flash board

- Connect keyboard to computer
- Press physical RESET button on bottom of keyboard
- Run the following commands:

```
  sudo dfu-programmer atmega32u4 erase
  sudo dfu-programmer atmega32u4 flash path/to/van/config/file.hex
  sudo dfu-programmer atmega32u4 start
```

- Enjoy!
