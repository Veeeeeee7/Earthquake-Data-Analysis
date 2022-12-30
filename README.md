# Earthquake Data Analysis

### Made for engineering class.

To use this, add the all data files _(.csv only)_ in the `./data` folder. Each data file should have 3 columns: `Time (s)`, `A-output`, `B-output`. The program will then convert each data file into `.wav` files, located in `./wav files`. The frequency is then found using these files through a Fast Fourier Transform and Autocorrelation. The program will then output the frequency in Hz. The frequency might be different for the two methods, usually one is correct so pick the one that seems more reasonable. _ie do not pick the one that is more than 10 Hz unless it somehow matches your data_. The program will also compute the maximum absolute value for each output, which is the maximum acceleration.

### Sample Data Output

    shortBuilding_40percent
    -----------------------------------------------------
    Analyzing A-output:
    Calculated frequency from FFT: 21.010745986491457 Hz
    Calculated frequency from autocorrelation: 2.10178694820381 Hz
    Maximum Acceleration: 0.57968

    Analyzing B-output:
    Calculated frequency from FFT: 2.0983606049885064 Hz
    Calculated frequency from autocorrelation: 0.5251127301130596 Hz
    Maximum Acceleration: 0.336365

<img width="500" src="imgs/graph.png">

Source: https://gist.github.com/endolith/255291
