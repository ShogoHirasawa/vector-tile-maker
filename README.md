# Generate Vector Tiles with Tippecanoe on Google Colab

This repository contains a Google Colab notebook (`.ipynb`) that demonstrates how to transform GeoJSON data into vector tiles using [Tippecanoe](https://github.com/mapbox/tippecanoe). Below you will find an overview of its purpose, as well as instructions for how to run it in Colab.

## Overview

1. **Tippecanoe Installation**  
   The notebook will clone the Tippecanoe repository from GitHub and build it within the Colab environment.

2. **GeoJSON Upload**  
   You can upload one or more GeoJSON files directly from your local machine to the Colab session.

3. **Vector Tile Generation**  
   The notebook runs Tippecanoe to produce `.pbf` tiles, organized into a folder structure.

4. **Download as ZIP**  
   Finally, the generated tiles can be zipped and downloaded, so you can host them or use them in your mapping application.

## Why Use This Notebook?

- **No Local Setup**: You do not need to install Tippecanoe or configure a development environment locally.
- **Rapid Experimentation**: Colab provides a ready-to-use environment, allowing you to quickly test and preview different zoom levels, layer names, or tile configurations.
- **Easy for Non-Engineers**: Users without a technical background can still create vector tiles simply by uploading GeoJSON files and running a few cells in the notebook.
- **Open-Source Workflow**: All steps are transparent and reproducible. Anyone with a Google account can copy this notebook, adapt it, and run it.

## How to Use

1. **Open the Notebook in Colab**  
   - Click on the “[Open in Colab](https://github.com/ShogoHirasawa/vectot-tile-maker/blob/main/vectorTileMaker.ipynb)” badge (if you have added one), or open the `.ipynb` file directly from this repo on GitHub and select “Open in Colab” (requires the [Colab Chrome extension](https://chrome.google.com/webstore/detail/open-in-colab/)).

2. **Run the Cells in Order**  
   - The first cell installs Tippecanoe by cloning and building the source code.
   - The second cell prompts you to upload your GeoJSON file(s).
   - The notebook automatically reads the filename, extracts the layer name, runs Tippecanoe, and produces a folder with the `.pbf` tiles.

3. **Download the Output**  
   - After the vector tiles are generated, the notebook zips them and provides a download link.

4. **Usage Notes**  
   - When you restart the Colab environment, you must re-run the notebook cells to rebuild Tippecanoe and re-upload your files.
   - Ensure that your GeoJSON data is properly formatted; Tippecanoe can be sensitive to invalid geometries.

## Repository Contents

- **`vectorTileMaker.ipynb`**  
  The main Colab notebook, containing all steps for installing Tippecanoe and generating tiles.  
- **`README.md`**  
  This file, providing an overview of how to get started and run the notebook.

## Contributing

Feel free to open issues or submit pull requests if you find any bugs or have suggestions on how to improve the workflow. Contributions are always welcome!

## License

This repository is distributed under the [MIT License](LICENSE). See `LICENSE` for more information.
