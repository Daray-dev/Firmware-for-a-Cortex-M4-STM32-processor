# Firmware-for-a-Cortex-M4-STM32-processor
 building bare-metal firmware for a Cortex-M4 STM32 microcontroller, using open source tools and libraries such as GCC and libopencm3. The project will cover everything from blinking an LED, to building a bootloader for performing firmware updates over UART/USB, to building a signed firmware security mechanism that allow only authorised code to run on the device. Stretch goal content includes *breaking* the security we build, as well as exploring more peripherals, applications, and algorithms in depth.

 ## Repo setup

```bash
# Clone the repo
git clone git@github.com:lowbyteproductions/bare-metal-series.git
cd bare-metal-series

# Initialise the submodules (libopencm3)
git submodule init
git submodule update

# Build libopencm3
cd libopencm3
make
cd ..

# Build the bootloader firmware
cd bootloader
make
cd ..

# Build the main application firmware
cd app
make
```
