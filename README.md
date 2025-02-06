# **Multispectral Image Processing Toolbox**

## **Overview**
The **Multispectral Image Processing Toolbox** is an open-source Python framework designed for processing aerial multispectral imagery to monitor mistletoe species in urban parks. This project facilitates image organization, spectral calibration, geometric alignment, feature extraction, and data storage, ensuring accurate and efficient analysis of remote sensing data.

## **Features**
- **Co-registration and Geometric Alignment**: Ensures spatial alignment across spectral bands and multiple image captures.
- **Spectral Calibration**: Converts raw sensor data into calibrated reflectance values.
- **Feature Extraction**: Computes vegetation indices and texture features for mistletoe detection.
- **Data Storage & Management**: Organizes, processes, and exports data in GIS-compatible formats.
- **Automated Processing Pipeline**: Streamlines image preprocessing, calibration, and feature engineering.

## **Project Structure**

The project follows a modular structure for efficient organization and development. See the **[Project Structure Guide](generate_project_struct.txt)** for further details.

```
Multispectral_Image_Processing_Toolbox/
├── project_docs/
│   ├── project_outline.md
│   ├── project_outline_technical.md
│   ├── glossary.md
│   ├── glossary_technical.md
│   ├── librarys.md
│
├── src/
│   ├── data_ingestion/
│   ├── spectral_calibration/
│   ├── geometric_alignment/
│   ├── feature_extraction/
│   ├── data_storage/
│
├── tests/
├── data/
├── notebooks/
├── docs/
├── scripts/
```

## **Installation**
For setup and installation instructions, refer to the **[Installation Guide](docs/installation_guide.md)**.

## **Documentation**
- **[Project Outline](project_docs/project_outline.md)**: High-level project objectives, tasks, and expected impact.
- **[Technical Outline](project_docs/project_outline_technical.md)**: Detailed breakdown of processing modules, technical considerations, and pipeline workflows.
- **[General Glossary](project_docs/glossary.md)**: Definitions of core remote sensing and image processing concepts.
- **[Technical Glossary](project_docs/glossary_technical.md)**: Advanced definitions related to spectral analysis and geospatial data.
- **[Library Reference Guide](project_docs/librarys.md)**: Overview of Python libraries used in each module.

## **Core Modules**
Each major component of the toolbox is implemented as a separate module. More details are available in the **[Technical Outline](project_docs/project_outline_technical.md)**.

### **1. Data Ingestion & Preprocessing**
- Organizes files and extracts metadata.
- Libraries: `pathlib`, `glob`, `piexif`, `pyexiftool`.
- Code: `src/data_ingestion/file_manager.py`, `src/data_ingestion/metadata_extractor.py`.

### **2. Spectral Calibration & Alignment**
- Applies reflectance corrections and geometric transformations.
- Libraries: `rasterio`, `py6S`, `numpy`, `opencv-python-headless`.
- Code: `src/spectral_calibration/reflectance_calc.py`, `src/spectral_calibration/atmospheric_correction.py`.

### **3. Feature Extraction**
- Computes vegetation indices and texture-based features.
- Libraries: `scikit-image`, `spectral`, `scipy`.
- Code: `src/feature_extraction/spectral_features.py`, `src/feature_extraction/texture_analysis.py`.

### **4. Data Storage & Export**
- Stores processed data in GIS-compatible formats.
- Libraries: `rasterio`, `SQLAlchemy`, `h5py`, `boto3`.
- Code: `src/data_storage/storage_manager.py`, `src/data_storage/database_handler.py`.

### **5. System Integration & Automation**
- Automates data processing workflows.
- Libraries: `argparse`, `logging`, `Dask`, `joblib`.
- Code: `src/pipeline/pipeline_manager.py`, `src/pipeline/logging_config.py`.

## **Development Timeline**
| **Task** | **Estimated Duration** |
|----------|--------------------|
| Data Ingestion & Preprocessing | 1-2 weeks |
| Spectral Calibration & Reflectance Correction | 2-4 weeks |
| Geometric Co-Registration | 4-7 weeks |
| Feature Extraction (Spectral & Texture Analysis) | 7-10 weeks |
| Data Storage & Output Management | 7-10 weeks (parallel) |
| System Integration & Pipeline Automation | 10-12 weeks |

## **Contributions**
Contributions are welcome! Please refer to the **[Developer Guide](docs/developer_guide.md)** for guidelines on extending and modifying the toolbox.

## **License**
This project is licensed under the **MIT License**. See **[LICENSE](LICENSE)** for more details.

## **Contact & Support**
For support or inquiries, refer to the **[FAQ](docs/faq.md)** or reach out via GitHub issues.

