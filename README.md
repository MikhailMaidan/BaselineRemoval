# BaselineRemoval
Script correct the basseline via 2 different methods
This Python script performs baseline correction on a set of spectra data files in the Glucose_200 folder. The baseline correction is applied using two methods: ModPoly and IModPoly, each with different polynomial degrees (2, 3, and 4). The script uses the BaselineRemoval library to perform the baseline correction.

The script reads each spectrum data file (in .txt format) from the Glucose_200 folder and processes it one by one. It applies baseline correction for each method and polynomial degree combination and saves the processed data to an output Excel file.

After processing each spectrum, the script generates plots for each baseline correction method and polynomial degree combination. The plots show the original spectrum, the baseline-removed spectrum (using the respective method and degree), and the baseline-corrected spectrum. Each plot is limited to the range of wavenumbers between 900 and 1900 (1/cm). The plots are saved in the 'processed_data_glucose_200_cut_spectra_slaves' folder.

The script defines a function called process_file, which takes the file path of a spectrum and the output folder as input. The function reads the data, performs baseline correction using the specified methods and degrees, saves the processed data to an Excel file, and generates the plots.

The main function is the entry point of the script. It checks if the output folder exists; if not, it creates the folder. Then, it processes each text file in the Glucose_200 folder, one by one, using the process_file function.

The purpose of this script is to preprocess and visualize the spectra data by applying baseline correction using different methods and polynomial degrees. The resulting processed data and plots can be further analyzed to study the spectral features of the Glucose_200 samples.
