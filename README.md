# Geo Data Viewer

## Overview
Geo Data Viewer is a __VS Code extension__ designed for viewing and analyzing geospatial data directly within the editor. It supports common geospatial formats, including __GeoJSON__, __CSV__ (with latitude/longitude), and __Shapefiles__, providing a lightweight alternative to traditional GIS software.

This extension is particularly useful for users who work with geospatial data in a coding environment, enabling quick visualization and basic exploration without requiring external applications.

(have a preview of the geo-data-viewer)

## Features
### ✅ Supported Data Formats
- __📍 GeoJSON__ – Standard format for geographic data.
- __📊 CSV__ – Requires lat/lon columns.
- __🗂 Shapefiles__ – Requires appropriate handling.

### ⚡ Functionality
- __🗺 Interactive Map View__ – Visualize geospatial data directly in VS Code.
- __🔍 Attribute Inspection__ – Explore properties of geographic features.
- __🚀 Lightweight & Fast__ – No need for bulky GIS software.


## 📌 Installation  
To install **Geo Data Viewer**, follow these steps:  

1. Open **VS Code**.  
2. Go to the **Extensions Marketplace** (`Ctrl + Shift + X` / `Cmd + Shift + X`).  
3. Search for **Geo Data Viewer**.  
4. Click **Install**.  

Alternatively, install via the **command line**:  

```sh
code --install-extension geo-data-viewer
```

(import a install gif)


## Usage
### `View Map`: `ctrl`/cmd + alt + m)
### `View Map from Url`:
### `Map Gallery`: 

Opening a Geospatial File
### Viewing Data on a Map

Run Geo: View Map (ctrl/cmd + alt + m) command on an open geo data document to view 🗺️
Use Geo: View Map from Url (ctrl/cmd + alt + u) command to load a map from kepler.gl demo app, github repository, or a gist
Run Geo: Map Gallery (ctrl/cmd + alt + g) command to view a list of built-in public keplergl map configs 🗺️


## Example


### - 🗺️ Example 1: Open & Visualize Geospatial Data
📌 **How to open a geospatial file and display it on a map**  

✅ **Steps:**  
1. Open `world_cities.geojson` in **VS Code**.  
2. Right-click → **"Geo: View Map"**.  
3. The map will load, displaying **city markers**.

### - 🔍 Example 2: Inspect Feature Properties
**How to click on map features to explore their attributes**



### - 🎨 Example 3: Customize Map Style & Visualization


