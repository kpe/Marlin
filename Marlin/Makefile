### DISCLAIMER
### This Makefile is for use with the 2014 Series-1 and arduino-mk.  
### see instructions for installation and use at forum.typemachines.com
### For detailed explanations about all the avalaible options,
### please refer to https://github.com/sudar/Arduino-Makefile/blob/master/arduino-mk-vars.md

### PROJECT_DIR
### This is the path to where you have created/cloned your project
PROJECT_DIR       =/home/kpe/proj/local/Marlin/Marlin

### ARDMK_DIR
### Path to the Arduino-Makefile directory.
ARDMK_DIR         = /home/kpe/proj/local/Arduino-Makefile

### ARDUINO_DIR
### Path to the Arduino application and ressources directory.
ARDUINO_DIR       = /home/kpe/opt/arduino/arduino

ARDUINO_LIBS      = Wire LiquidCrystal SPI

### USER_LIB_PATH
### Path to where the your project's libraries are stored.
USER_LIB_PATH     :=  $(PROJECT_DIR)/lib

### BOARD_TAG
### It must be set to the board you are currently using. (i.e uno, mega2560, etc.)
BOARD_TAG         = mega2560

### MONITOR_BAUDRATE
### It must be set to Serial baudrate value you are using.
#MONITOR_BAUDRATE  = 115200
MONITOR_BAUDRATE  = 115200

### AVR_TOOLS_DIR
### Path to the AVR tools directory such as avr-gcc, avr-g++, etc.
AVR_TOOLS_DIR     = /usr

### AVRDDUDE
### Path to avrdude directory.
AVRDUDE          = /home/kpe/opt/arduino/bin/avrdude
AVRDUDE_CONF     = /home/kpe/opt/arduino/etc/avrdude.conf


### CPPFLAGS
### Flags you might want to set for debugging purpose. Comment to stop.
#CPPFLAGS         = -pedantic -Wall -Wextra
CPPFLAGS         =  -Wall -Wextra

### MONITOR_PORT
### The port your board is connected to. Using an '*' tries all the ports and finds the right one.
MONITOR_PORT      = /dev/ttyACM*
MONITOR_CMD      = picocom

### don't touch this
CURRENT_DIR       = $(shell basename $(CURDIR))

### OBJDIR
### This is were you put the binaries you just compile using 'make'
OBJDIR            = $(PROJECT_DIR)/bin/$(BOARD_TAG)/$(CURRENT_DIR)

VARIANT = mega
F_CPU = 16000000L

### path to Arduino.mk, inside the ARDMK_DIR, don't touch.
include $(ARDMK_DIR)/Arduino.mk
