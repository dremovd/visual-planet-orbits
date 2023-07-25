# Solar System Planet Tracker

This project visualizes the position and distance of the planets in our solar system with respect to Earth, from the start of 2023 to the end of 2025.

## Dependencies

- Python 3.8 or above
- Matplotlib
- Seaborn
- Skyfield
- IPython
- Numpy
- FFMPEG

To install these Python libraries, use pip:

```bash
pip install matplotlib seaborn skyfield ipython numpy
```
You'll also need FFMPEG for video creation. Installation depends on your OS, but you can find instructions on the official website: [FFMPEG](https://www.ffmpeg.org/download.html).

## How it Works

The script uses the Skyfield library to compute positions of planets in our solar system. It creates a plot for each day between January 1, 2023 and December 31, 2025, showing:

- The relative positions of each planet to the Sun, with the distances marked.
- The time-series plot of each planet's distance to Earth.

After creating the daily plots, it saves them as PNG images.

At the end, it uses FFMPEG to compile these images into an mp4 video, providing a time-lapse view of the solar system.

## Usage

1. Clone this repository.
2. Open Jupyter Notebook or Jupyter Lab on your machine.

    If you do not have Jupyter installed, you can install it via pip:

    ```bash
    pip install jupyterlab
    ```

3. Navigate to the directory where you cloned the repository.
4. Open the .ipynb file in Jupyter.
5. Run the entire notebook by clicking on the "Kernel" menu, then "Restart & Run All".

This script will create an mp4 file named "planets.mp4" in the same directory as the notebook.

## Notes

- The Jupyter Notebook may take some time to run due to the complexity of the computations and the number of plots that are generated.
- Ensure that you have enough disk space for the generated plots and the mp4 video file. The file size will depend on the duration of the period being plotted.

## License

This project is licensed under the terms of the MIT license.
