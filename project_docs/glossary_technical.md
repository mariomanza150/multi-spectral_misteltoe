# **Multispectral Image Processing Toolbox - Technical Glossary**

## **Table of Contents**

### **1. Advanced Image Processing & Spectral Analysis**
- [Radiometric Correction](#radiometric-correction)
- [Spectral Response Function](#spectral-response-function)
- [Bidirectional Reflectance Distribution Function (BRDF)](#bidirectional-reflectance-distribution-function-brdf)
- [Spectral Calibration](#spectral-calibration)
- [Spectral Bands](#spectral-bands)

### **2. Geospatial Data & Remote Sensing**
- [Ground Sampling Distance (GSD)](#ground-sampling-distance-gsd)
- [Geospatial Data Structures](#geospatial-data-structures)
- [Coordinate Reference Systems (CRS)](#coordinate-reference-systems-crs)
- [Geometric Transformations](#geometric-transformations)
- [Homography Transformation](#homography-transformation)

### **3. Vegetation Analysis & Environmental Monitoring**
- [Leaf Area Index (LAI)](#leaf-area-index-lai)
- [Soil Adjusted Vegetation Index (SAVI)](#soil-adjusted-vegetation-index-savi)
- [Canopy Reflectance Models](#canopy-reflectance-models)
- [Radiative Transfer Model (RTM)](#radiative-transfer-model-rtm)
- [Mistletoe Spectral Signatures](#mistletoe-spectral-signatures)

---

## **1. Advanced Image Processing & Spectral Analysis**

### **Radiometric Correction**
**Definition:** The process of adjusting image pixel values to compensate for sensor irregularities and environmental influences, ensuring accurate spectral reflectance values.
**Formula:**
\[
R_{corr} = \frac{L - L_{dark}}{E}\times G
\]
where:
- \( L \) = Radiance
- \( L_{dark} \) = Dark object subtraction term
- \( E \) = Irradiance
- \( G \) = Gain factor
**Use Case:** Applied in multispectral imaging to standardize reflectance values across varying light conditions.

### **Spectral Response Function**
**Definition:** A function describing the sensitivity of an imaging sensor to different wavelengths.
**Implementation:** Used to correct sensor bias when processing multispectral and hyperspectral data.

### **Bidirectional Reflectance Distribution Function (BRDF)**
**Definition:** A function describing how light is reflected at different angles from a surface.
**Equation:**
\[
BRDF(\theta_i, \theta_r, \phi) = \frac{L_r(\theta_r, \phi)}{E_i(\theta_i)}
\]
where:
- \( \theta_i, \theta_r \) = Incident and reflected angles
- \( \phi \) = Azimuth angle
**Use Case:** Used to model anisotropic reflectance for vegetation and terrain analysis.

### **Spectral Calibration**
**Definition:** The process of correcting spectral distortions due to sensor limitations.
**Implementation:** Typically performed using reference calibration targets and empirical line correction.

### **Spectral Bands**
**Definition:** Discrete wavelength ranges captured by an imaging sensor.
**Application:** Used in vegetation indices like NDVI and SAVI.

---

## **2. Geospatial Data & Remote Sensing**

### **Ground Sampling Distance (GSD)**
**Definition:** The real-world distance represented by each pixel in a remotely sensed image.
**Formula:**
\[
GSD = \frac{H \times p}{f}
\]
where:
- \( H \) = Sensor altitude
- \( p \) = Pixel size
- \( f \) = Focal length
**Use Case:** Essential for determining image resolution in aerial surveys.

### **Geospatial Data Structures**
**Definition:** Data models used to store and process geographic information.
**Types:** Raster and vector models.

### **Coordinate Reference Systems (CRS)**
**Definition:** A system used to define spatial coordinates in mapping applications.
**Example:** WGS 84 is a commonly used CRS for global positioning.

### **Geometric Transformations**
**Definition:** Mathematical operations used to align and correct images.
**Example:** Used in image co-registration for aligning spectral bands.

### **Homography Transformation**
**Definition:** A transformation matrix used to project an image onto another plane.
**Use Case:** Applied in co-registration of multispectral images for accurate feature matching.

---

### **Spectral Data Noise Sources**
**Definition:** Various environmental and sensor-related factors that introduce inaccuracies or distortions in multispectral data.

**Types of Noise:**
- **Cloud Cover & Atmospheric Disturbances:** Partially or fully obstructs the Earth's surface, affecting spectral readings and requiring cloud-masking techniques.
- **Sensor Drift & Calibration Errors:** Variations in sensor sensitivity over time can introduce measurement biases.
- **Aerosol & Water Vapor Interference:** Scattering and absorption of light by atmospheric particles lead to spectral distortions, requiring radiometric corrections.
- **Illumination Variability:** Changes in solar angle and shadows cast by terrain features affect reflectance values.

**Use Case:** Implementing **radiometric corrections** and **cloud-masking algorithms** to enhance data accuracy in multispectral analysis.

---

### **Aerial Survey Limitations**
**Definition:** The constraints and challenges associated with acquiring aerial multispectral imagery, particularly when using drones or satellites. 

**Key Factors:**
- **Regulatory Restrictions:** Aviation laws may limit drone altitude, flight times, and no-fly zones, particularly in urban areas.
- **Weather Conditions:** Wind, rain, and cloud cover can interfere with stable image acquisition and affect spectral consistency.
- **Battery Life & Range:** Drones have limited operational endurance, restricting the size of survey areas per flight.
- **Data Resolution Trade-offs:** Higher resolution imagery requires lower altitudes and slower speeds, reducing the coverage per flight session.

**Use Case:** Planning optimal flight paths and scheduling data collection during favorable weather conditions to ensure consistent image quality and spectral integrity.

---

## **3. Vegetation Analysis & Environmental Monitoring**

### **Leaf Area Index (LAI)**
**Definition:** A dimensionless value representing the total leaf area per unit ground area.
**Application:** Used in ecosystem modeling and carbon cycle studies.

### **Soil Adjusted Vegetation Index (SAVI)**
**Definition:** A modified vegetation index that accounts for soil brightness in arid environments.
**Formula:**
\[
SAVI = \frac{(NIR - Red) \times (1 + L)}{(NIR + Red + L)}
\]
where \( L \) is a soil brightness correction factor.
**Use Case:** Used in dryland agriculture and forestry applications.

### **Canopy Reflectance Models**
**Definition:** Models describing how light interacts with vegetation canopies.
**Application:** Used in remote sensing to estimate plant health and biomass.

### **Radiative Transfer Model (RTM)**
**Definition:** A mathematical model describing light interactions with the atmosphere and vegetation.
**Implementation:** Used in atmospheric correction for multispectral images.

### **Mistletoe Spectral Signatures**
**Definition:** Unique spectral reflectance patterns associated with mistletoe species.
**Use Case:** Used in remote sensing to detect mistletoe infestations in urban parks.

---

## **Quick Reference: Project Outline Connection**
The **Multispectral Image Processing Toolbox** includes several advanced processing steps requiring these technical concepts:
- **Preprocessing & Calibration:** [Radiometric Correction](#radiometric-correction), [Spectral Calibration](#spectral-calibration)
- **Geometric Alignment:** [Homography Transformation](#homography-transformation), [Geometric Transformations](#geometric-transformations)
- **Feature Extraction:** [Leaf Area Index (LAI)](#leaf-area-index-lai), [SAVI](#soil-adjusted-vegetation-index-savi), [Canopy Reflectance Models](#canopy-reflectance-models)

For high-level explanations, see the [General Glossary](glossary.md).

