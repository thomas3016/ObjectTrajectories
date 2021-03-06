# SSD
The code is situated in the `src` folder. The folder `trained_models` should instead contain the SSD Model (weights).

The main script is `SSDVideo.py`

Basic usage:

`$ python3 SSDVideo.py -i <InputFolder> -o <OutputFolder>`

The input folder should be a directory containing sequential images corresponding to video frames of the dataset.

Other arguments can be used:

`$ python3 SSDVideo.py -i <InputFolder> -o <OutputFolder> [ -m <PathToWeights> ] [ -ox <PathToOxtsFolder> ] [ -ts <PathToTimestampsFile> ]`

Data is stored in a Python data structure and are saved in a pickle file in order to be used also in subsequent operations 

Trajectories can be shown graphically usin the script `plot.py`. It doesn't require any argument and it uses the pickle files generated by the `SSDVideo.py` script.
To advance, press any key. One step corresponds to a video frame.
In the plot each color represents a different unique object detected.
