# EBVCubeVisualizerPlugin                                                 <img align="left" src="https://github.com/E-O-Conchas/EBVCubeVisualizerPlugin/blob/master/EBVIcon.png" alt="drawing" width="50"/>      

**EBVCubeVisualizerPlugin** is a QGIS plugin designed for visualizing Essential Biodiversity Variables (EBVs) stored in the [EBV Data Portal](https://portal.geobon.org/datasets) as EBVCube netCDF files. The plugin allows users to select and display specific slices of EBV data cubes based on time, entity, scenario, and metric, providing a flexible and powerful tool for biodiversity analysis.

## Features

- Load and visualize EBVCube data stored in netCDF files.
- Subset data by time, entity, scenario, and metric.
- Automatically apply the correct Coordinate Reference System (CRS) based on the netCDF file metadata.
- Display the selected data on the QGIS canvas with clear layer names that include entity and time information.

## Installation

1. Download this repository as zip file.
2. Open QGIS and go to `Plugins > Manage and Install Plugins...`.
3. Click on `Install from ZIP` and select the downloaded file.
4. Activate the plugin by checking the box next to "EBVCubeVisualizerPlugin" in the `Installed` tab.

## Usage

1. **Open the Plugin:**
   - After installation, go to `Plugins > EBVCubeVisualizerPlugin` to open the plugin interface.

2. **Load a netCDF File:**
   - Use the file browser to select a netCDF file containing EBVCube data.

3. **Select Parameters:**
   - Choose the desired `Entity`(e.g., species), `Time`(e.g., year), `Metric` (e.g., Biodiversity metric) and `Scenario` (e.g., SSP1) from the dropdown menus.

4. **Visualize Data:**
   - Click the `Add Layer` button to display the selected subset of data on the QGIS canvas. The layer will be styled with an automatically generated color ramp base on the data values.

5. **Customize Visualization:**
   - Use QGIS layer properties to further customize the visualization, such as adjusting the color scheme or applaying spatial analysis tools.

## Dependencies

- QGIS 3.0 or later
- Python 3.6 or later
- Required Python Libraries:
  - `netCDF4`: Handles netCDF file loading and data extraction.
  - `numpy`: Supports array operations and data handling.
  - `gdal`: Facilitates raster data management and processing.

## Troubleshooting

If you encounter any issues with the plugin, please follow these steps:

1. Ensure that all dependencies are installed and correctly configured.
2. Verify that the netCDF file you are using is properly formatted and contains the required dimensions (e.g., `entity`, `time`, `lat`, `lon`).
3. Check the QGIS Python console for any error messages and provide them when seeking help.

## Contributing

We welcome contributions to this project! If you have an idea for a new feature or have found a bug, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Future Enhancements
- **User Interface Improvements:** Streamline the interface for easier parameter selection and data visualization.
- **Data availability:** Provide the catalog of the EBV portla within the plug-in if possible
Stay tuned for future updates and enhancements!

