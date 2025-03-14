# Geo Data Viewer

## Overview
Geo Data Viewer is a __VS Code extension__ designed for viewing and analyzing geospatial data directly within the editor. It supports common geospatial formats, including __GeoJSON__, __CSV__ (with latitude/longitude), and __Shapefiles__, providing a lightweight alternative to traditional GIS software.

This extension is particularly useful for users who work with geospatial data in a coding environment, enabling quick visualization and basic exploration without requiring external applications.

(have a preview img for the geo-data-viewer)

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
2. Go to the **Extensions Marketplace** (`ctrl + shift + x` / `cmd + shift + x`).  
3. Search for **Geo Data Viewer**.  
4. Click **Install**.

(import a install gif)



## Usage
### 🚀 1️⃣ Open a Geospatial File and View It on a Map
- Open a **geo data file** (e.g., `.geojson`, `.shp`, `.kml`, etc.) in **VS Code**.
- Run the **"View Map"** command to visualize the data:
  - **Shortcut:** `Ctrl + Alt + M` (Windows/Linux) or `Cmd + Alt + M` (Mac).
  - This will open an interactive map displaying the geo data. 🗺️
  - **Example:** 

### 🔗 2️⃣ Load a Map from a URL
- You can also load a map from external sources such as:
  - A **[Kepler.gl demo app](https://kepler.gl/demo?mapUrl=https://gist.githubusercontent.com/JesperDramsch/73a2f437cfc1e6e968cddfbb4793167f/raw/66550b932db2a93a495b3e362309e676b084991b/expat_keplergl.json)**.
  - A **GitHub repository**.
  - A **[GitHub Gist](https://gist.github.com/search?l=JSON&q=keplergl)**.

- To do this, run the **"View Map from URL"** command:
  - **Shortcut:** `Ctrl + Alt + U` (Windows/Linux) or `Cmd + Alt + U` (Mac).
  - **Example:** 


### 🗺️ 3️⃣ Explore the Map Gallery
- The **Map Gallery** provides a collection of built-in **public Kepler.gl map configurations**.
- To open the gallery, run the **"Geo: Map Gallery"** command:
  - **Shortcut:** `Ctrl + Alt + G` (Windows/Linux) or `Cmd + Alt + G` (Mac).
  - Browse and load pre-configured maps for easy exploration.
  - **Example:**  

