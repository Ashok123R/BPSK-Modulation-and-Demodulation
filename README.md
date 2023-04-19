# BPSK-Modulation-and-Demodulation
BPSK Modulation and Demodulation
The aim of the simulation is to reconstruct a transmitted image, modulated by BPSK scheme, at
the receiver. The maximum likelihood decoder will be used at the receiver to recover the symbols. To
model a channel for transmission AWGN noise will be added to transmitted signal before processing
at the receiver. The bit error rate (BER) vs SNR(in dB) curve will be plotted for different values
of SNR and will be compared with the theoretical value. Note that we are a using the baseband
transmission for simulation.
Following are the steps to be followed for the simulation experiment.
1. Read the image cameraman.png. You can get the image by clicking here. The image is of size
256 × 256. Use suitable python package for reading the image (imageio, opencv etc).
2. Convert the pixel values to bits and map to BPSK symbols. Make sure to use same number
of bits for all the values. Plot the constellation diagram of the BPSK symbols.
3. Set an SNR value for the transmission and generate a complex Gaussian noise with enough
number of samples for the required SNR.
4. The received signal which is the combination of BPSK symbol and the noise samples shall
be passed through an ML decoder to do the demapping. The constellation diagram of the
received signal shall be plotted.
1
5. Convert the demapped symbols to bits and then to pixel values. Also find the BER.
6. Reconstruct the image.
7. Iterate the above steps for SNR (in dB) values from -10 to 10 with increments of 1 and plot
the BER. Also plot the theoretical BER value for BPSK Modulation. Compare them.
