# ArcGIS Online Credit Cost Estimator

A lightweight web-based tool to estimate ArcGIS Online credit costs for hosting feature data, tiled imagery, and common GIS file types. This tool is designed for GIS analysts and teams to better understand and manage hosting costs on ArcGIS Online.


## Features
- **Manual Input**: Calculate credit costs for feature hosting (in MB) and tiled imagery hosting (in GB) based on user-provided file sizes.
- **File Upload**: Upload common GIS data files (e.g., `.tif`, `.gdb`, `.csv`, `.xls`, `.xlsx`) to calculate credit costs based on file size and type.
- **Real-Time Feedback**: Instantly see estimated credit costs after entering values or uploading files.
- **Web-Based**: Accessible via any modern web browser—no software installation required.

## Supported File Types
| File Type       | Description                  | Hosting Cost Logic                         |
|------------------|------------------------------|-------------------------------------------|
| `.tif`          | Tiled imagery data           | Imagery hosting rate: 1.2 credits/GB       |
| `.gdb`          | Geodatabase files            | Feature hosting rate: 2.4 credits/10 MB    |
| `.csv`, `.xls`, `.xlsx` | Tabular data files    | Feature hosting rate: 2.4 credits/10 MB    |

## Live Demo
Access the live version of this tool hosted on GitHub Pages:
[ArcGIS Online Credit Cost Estimator](https://yourusername.github.io/arcgis-credit-calculator-web)

## How It Works
1. **Manual Input**:
   - Enter the size of your data in MB or GB.
   - Click "Calculate Cost" to see the estimated credits required for hosting.

2. **File Upload**:
   - Upload a GIS data file.
   - The tool automatically calculates the file size and provides an estimated hosting cost based on the file type.

3. **Dynamic Calculations**:
   - Cost estimation is based on Esri's standard pricing model:
     - **Feature Hosting**: 2.4 credits per 10 MB per month.
     - **Tiled Imagery Hosting**: 1.2 credits per GB per month.

## Setup and Development
### Prerequisites
- A modern web browser (Chrome, Firefox, Edge, Safari, etc.)

### Local Usage
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/arcgis-credit-calculator-web.git
