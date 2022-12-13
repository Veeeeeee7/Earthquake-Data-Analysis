# Frequency Finder

### Made for engineering class.

To use this, add the data as a csv file titled `data.csv` in the same directory as the python file. The data should have 3 columns: `Time (s)`, `A-output`, `B-output`. The program will then convert the `data.csv` file into two separate files: `A-output.wav` and `B-output.wav`. The frequency is then found using these `.wav` files through a Fast Fourier Transform and Autocorrelation. The program will then output the frequency in Hz. The frequency might be different for the two methods, usually one is correct so pick the one that seems more reasonable. _ie do not pick the one that is more than 10 Hz unless it somehow matches your data_
