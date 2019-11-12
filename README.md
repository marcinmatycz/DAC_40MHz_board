# DAC_40MHz_board
40MHz clock, 15MHz bandwith DAC board

This is a PCB board with LTC1667 14-bit digital-to-analog converter, designed for university assingment.
Parameters:
- supply voltage: +/-5V,
- 40MHz input clock,
- 15MHz bandwith,
- output signal level: +/-2V,
- 50Ω asymmetrical SMA output.

5th order Chebyshev passive filter was designed with rf-tools.com/lc-filter and normalized to standard, available values.
ADA4807 operational amplifier was chosen for first stage differential to single--ended amplifier because of bandwith and reasonable slew rate, capable of driving +-2V output at 15MHz. LT1809 was chosen for second stage non-inverting amplifier because of rail-to-rail output, good slew rate and high output current, so it could drive +-4V on 50 ohm output resistance in series with 50 ohm load resistance.

