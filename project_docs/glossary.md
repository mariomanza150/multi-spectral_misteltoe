# **Multispectral Image Processing Toolbox - General Glossary**

## **Table of Contents**

### **1. Core Concepts**
- [Multispectral Imaging](#multispectral-imaging)
- [Hyperspectral Imaging](#hyperspectral-imaging)
- [Reflectance](#reflectance)
- [Remote Sensing](#remote-sensing)
- [Georeferencing](#georeferencing)
- [Calibration](#calibration)

### **2. Image Processing & Spectral Analysis**
- [Normalization](#normalization)
- [Dimensionality Reduction](#dimensionality-reduction)
- [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
- [Gray-Level Co-occurrence Matrix (GLCM)](#gray-level-co-occurrence-matrix-glcm)

### **3. Geospatial Data & Remote Sensing**
- [GeoTIFF](#geotiff)
- [Raster Data](#raster-data)
- [Vector Data](#vector-data)
- [Spatial Database](#spatial-database)

### **4. Environmental Monitoring & Vegetation Analysis**
- [Vegetation Index](#vegetation-index)
- [Radiative Transfer Model](#radiative-transfer-model)
- [Transformation Matrix (Homography)](#transformation-matrix-homography)

## **1. Core Concepts**

### **Multispectral Imaging**
**Definition:** Capturing images at multiple specific wavelength bands, typically 3-20, to analyze different material properties.
**Example:** Used in agriculture to monitor crop health by detecting chlorophyll levels in plants.
**See also:** [Hyperspectral Imaging](#hyperspectral-imaging) for more advanced spectral analysis.

### **Hyperspectral Imaging**
**Definition:** Capturing hundreds of narrow spectral bands for detailed material identification.
**Example:** Used in mineral exploration and environmental studies to differentiate surface compositions.

### **Reflectance**
**Definition:** The proportion of incident light that a surface reflects at different wavelengths.
**Example:** A healthy plant reflects more near-infrared (NIR) light compared to an unhealthy one, which is the basis for vegetation indices like NDVI.

### **Remote Sensing**
**Definition:** The process of acquiring data about Earth's surface using airborne or spaceborne sensors.
**Example:** Satellites capturing land cover changes over time for climate monitoring.

### **Georeferencing**
**Definition:** Assigning real-world coordinates to pixels in an image to align it with maps.
**Example:** Aerial images of Mexico City parks are georeferenced to study mistletoe species distribution.

### **Calibration**
**Definition:** Adjusting raw sensor data to ensure accuracy in spectral measurements.
**Example:** Correcting multispectral images for sensor biases and atmospheric effects.

## **2. Image Processing & Spectral Analysis**

### **Normalization**
**Definition:** Adjusting pixel values to a common scale for consistency across datasets.
**Example:** Used to correct lighting variations in multispectral images.

### **Dimensionality Reduction**
**Definition:** Techniques to reduce the number of spectral bands while retaining key information.
**Example:** PCA is used to reduce the complexity of hyperspectral data.

### **Principal Component Analysis (PCA)**
**Definition:** A statistical technique that transforms correlated variables into uncorrelated principal components, reducing data dimensionality.
**Example:** Helps in extracting significant spectral features for mistletoe detection.

### **Gray-Level Co-occurrence Matrix (GLCM)**
**Definition:** A statistical method to analyze texture by examining pixel intensity relationships.
**Example:** Used in remote sensing to differentiate vegetation species based on their texture properties.

## **3. Geospatial Data & Remote Sensing**

### **GeoTIFF**
**Definition:** A raster image format that embeds geospatial metadata for accurate location mapping.
**Example:** Used for storing multispectral images with spatial reference information.

### **Raster Data**
**Definition:** Grid-based spatial data representation commonly used in remote sensing.
**Example:** Elevation models and land cover maps are raster datasets.

### **Vector Data**
**Definition:** Geographic data represented as points, lines, or polygons.
**Example:** Used in GIS to map roads, buildings, and vegetation boundaries.

### **Spatial Database**
**Definition:** A database optimized for storing and querying geospatial data.
**Example:** PostGIS is a spatial database used to manage large-scale multispectral datasets.

## **4. Environmental Monitoring & Vegetation Analysis**

### **Vegetation Index**
**Definition:** A numerical value derived from spectral bands to assess vegetation properties.
**Example:** NDVI is a widely used index to measure plant health based on red and NIR reflectance.

### **Radiative Transfer Model**
**Definition:** A mathematical model describing how light interacts with the atmosphere and surface materials.
**Example:** Used for atmospheric correction in remote sensing applications.

### **Transformation Matrix (Homography)**
**Definition:** A matrix that aligns one image to another by correcting perspective distortions.
**Example:** Applied in image processing to co-register multispectral bands for precise analysis.

---
## **Quick Reference: Project Outline Connection**
The **Multispectral Image Processing Toolbox** is an open-source Python toolkit designed for **monitoring mistletoe species** in urban parks using aerial multispectral imagery. The glossary terms are directly related to key project components:
- **Co-Registration & Preprocessing:** [Georeferencing](#georeferencing), [Transformation Matrix (Homography)](#transformation-matrix-homography)
- **Spectral Calibration:** [Calibration](#calibration), [Reflectance](#reflectance), [Radiative Transfer Model](#radiative-transfer-model)
- **Feature Extraction:** [Vegetation Index](#vegetation-index), [GLCM](#gray-level-co-occurrence-matrix-glcm)
- **Data Management:** [GeoTIFF](#geotiff), [Spatial Database](#spatial-database)

For **detailed technical definitions**, see [Technical Glossary](glossary_technical.md).
