# Klipper_Ender3_PRO_BTT_SKR_MINI_E3_V2

Display Configuration
- https://github.com/teeminus/NoTouchScreenFirmware/wiki/Klipper-display-configuration

```
[display]
lcd_type: emulated_st7920
en_pin: EXP1_7
spi_software_sclk_pin: EXP1_6
spi_software_mosi_pin: EXP1_8
spi_software_miso_pin: PA3
encoder_pins: ^EXP1_5, ^EXP1_3
click_pin: ^!EXP1_2
```

Pin reference
- https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3/blob/master/hardware/BTT%20SKR%20MINI%20E3%20V2.0/Hardware/BTT%20SKR%20MINI%20E3%20V2.0-PIN.pdf

```
[stepper_z]
step_pin: PB0
dir_pin: PC5
enable_pin: !PB1
microsteps: 16
rotation_distance: 8
endstop_pin: probe:z_virtual_endstop
position_max: 250
```

```
[bltouch]
sensor_pin: ^PC14
control_pin: PA1
z_offset: 0

[safe_z_home]
home_xy_position: 110, 110 # Change coordinates to the center of your print bed
speed: 50
z_hop: 10                 # Move up 10mm
z_hop_speed: 5
```
