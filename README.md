# Geo Data Viewer

## Overview
Geo Data Viewer is a __VS Code extension__ designed for viewing and analyzing geospatial data directly within the editor. It supports common geospatial formats, including __GeoJSON__, __CSV__ (with latitude/longitude), and __Shapefiles__, providing a lightweight alternative to traditional GIS software.

This extension is particularly useful for users who work with geospatial data in a coding environment, enabling quick visualization and basic exploration without requiring external applications.

![Preview](https://raw.githubusercontent.com/Reproducible-Urban-Research/geo-data-viewer/main/media/geo-data-viewer-1.png)
![Preview](https://raw.githubusercontent.com/Reproducible-Urban-Research/geo-data-viewer/main/media/geo-data-viewer-2.png)

<br>

## Features
### ✅ Supported Data Formats
- __📍 GeoJSON__ – Standard format for geographic data.
- __📊 CSV__ – Requires lat/lon columns.
- __🗂 Shapefiles__ – Requires appropriate handling.

### ⚡ Functionality
- __🗺 Interactive Map View__ – Visualize geospatial data directly in VS Code.
- __🔍 Attribute Inspection__ – Explore properties of geographic features.
- __🚀 Lightweight & Fast__ – No need for bulky GIS software.

<br>

---

## 📌 Installation  
To install **Geo Data Viewer**, follow these steps:  

1. Open **VS Code**.  
2. Go to the **Extensions Marketplace** (`Ctrl + Shift + X` / `Cmd + Shift + X`).  
3. Search for **Geo Data Viewer**.  
4. Click **Install**.

![Installation Guide](https://raw.githubusercontent.com/Reproducible-Urban-Research/geo-data-viewer/main/media/Installation.gif)

<br>

---

## Usage
### 🚀 1️⃣ Open a Geospatial File and View It on a Map
- Open a **geo data file** (e.g., `.geojson`, `.shp`, `.kml`, etc.) in **VS Code**.
- Run the **"View Map"** command to visualize the data:
  - **Shortcut:** `Ctrl + Alt + M` (Windows/Linux) | `Cmd + Alt + M` (Mac).
  - This will open an interactive map displaying the geo data.
  - 📂 **Example: Viewing Underground Stations in London**  
    - You can obtain the Underground Stations in London dataset by:
      1. **Downloading it from OpenStreetMap's Overpass API**  
        - Follow the steps **[here](#how-to-download-geo-data)** to extract the data.
      2. **Downloading a ready-made dataset**  
        - [📂 Download Example Data](https://raw.githubusercontent.com/user/repository/main/london_stations.geojson)

![Guide](https://github.com/Reproducible-Urban-Research/geo-data-viewer/blob/main/media/example1_london_underground_stations_vs.gif)

<br>

### 🔗 2️⃣ Load a Map from a URL
- You can also load a map from external sources such as:
  - A **[Kepler.gl demo app](https://kepler.gl/demo?mapUrl=https://gist.githubusercontent.com/JesperDramsch/73a2f437cfc1e6e968cddfbb4793167f/raw/66550b932db2a93a495b3e362309e676b084991b/expat_keplergl.json)**.
  - A **GitHub repository**.
  - A **[GitHub Gist](https://gist.github.com/search?l=JSON&q=keplergl)**.

- To do this, run the **"View Map from URL"** command:
  - **Shortcut:** `Ctrl + Alt + U` (Windows/Linux) | `Cmd + Alt + U` (Mac).
  - **Example:** Loading a map from a raw GeoJSON URL.

[Guide](https://raw.githubusercontent.com/user/repository/main/sample.geojson) -- The link Guide doesn't work in my Geo Data Viewer.

<br>

### 🗺️ 3️⃣ Explore the Map Gallery
- The **Map Gallery** provides a collection of built-in **public Kepler.gl map configurations**.
- To open the gallery, run the **"Geo: Map Gallery"** command:
  - **Shortcut:** `Ctrl + Alt + G` (Windows/Linux) | `Cmd + Alt + G` (Mac).
  - Browse and load pre-configured maps for easy exploration.

![Installation Guide](https://github.com/Reproducible-Urban-Research/geo-data-viewer/blob/main/media/example3_mapgallery.gif)

<br>

---

## 📍 Example Queries & Sample Data
### 🚇 1️⃣ Underground Stations in London

#### 🔹 **How to Download Geo Data**
You can extract underground station data for London using **OpenStreetMap's Overpass API**.

### ✅ **Steps to Get the Data:**
1. Go to [Overpass Turbo](https://overpass-turbo.eu/).
2. Paste the following query into the Overpass Turbo query window:
   ```overpassql
   [out:json];
   area["name"="London"]->.searchArea;
   node["railway"="station"]["station"="subway"](area.searchArea);
   out body;
3. Click Run (▶) to execute the query.
4. Click Export and select GeoJSON format.
5. Download the GeoJSON file.

![Installation Guide](https://github.com/Reproducible-Urban-Research/geo-data-viewer/blob/main/media/example1_london_underground_stations.gif)
