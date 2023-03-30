# vga-simulator
Original VGA Simulator: https://www.ericeastwood.com/lab/vga-simulator/

Modified from [pvieito/VGASimulator.py](https://gist.github.com/pvieito/8cdb54a9a03fd36e51c8df6e331a3006)

## Prerequisites
- This project was tested on Python 3.11.2.
- Install dependencies:
```bash
pip install Pillow
```

# Setup
Paste the contents of `log_signals.vhdl` into your VGA core testbench file. 
The process will write a text file with timestamped signal values.

The default filename is `vga_out.txt`.

# Usage
Run `./vga_sim.py --help` for usage instructions.

## Example
To run a 640x480 @60Hz ([standard](http://tinyvga.com/vga-timing/640x480@60Hz)), run `./vga_sim.py vga_log.txt 640 480 25.175 48 33`

# Testing
To run unit tests, simply run `python3 -m unittest` in the root directory of the project.
Test discovery will automatically detect and run tests.

