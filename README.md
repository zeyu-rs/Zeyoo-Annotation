# Zeyoo Image Annotation Tool

A powerful and versatile image annotation software designed for both **general computer vision** and **remote sensing** applications.  
Supports **multiple annotation types**, **remote sensing geospatial data**, and **format conversions** for major AI and GIS workflows.

[Examples](https://github.com/zeyu-rs/Zeyoo-Annotation/blob/main/examples.md)

[Download1](https://ai4wild.com/zeyoo)

[Download2](https://github.com/zeyu-rs/Zeyoo-Annotation/releases)


## 🌟 Highlight Tips
1. Double-click to apply the target's color and other properties to the toolbar.  
2. Annotations are saved automatically when switching images. You can also press **Ctrl+S** to save manually.  
3. Supported input/output types (input formats can be auto-detected):  

| Type | Supported Input Formats | Default Output Format | Supported Convertible Output Formats |
|------|------------------------|-----------------------|---------------------------------------|
| Point | YOLO | YOLO | YOLO / Esri Shapefile / Image mask |
| Horizontal Bounding Box | YOLO / VOC / COCO | YOLO | YOLO / VOC / COCO / Esri Shapefile / Image mask |
| Oriented Bounding Box | DOTA / YOLO | DOTA | DOTA / YOLO /  Esri Shapefile / Image mask |
| Polygon | Labelme JSON / COCO / YOLO | Labelme JSON | COCO / YOLO / Esri Shapefile / Image mask |
| Polyline | Labelme JSON  | Labelme JSON |  Esri Shapefile / Image mask |

> **Note:** Input formats can be auto-detected.
> *Changelog — 2026-02-05 (v3.9.7)*  
>  
> - *Optimized focus mode.*
> - *Added class info display to show category and confidence on the image.*
> - *Added class info display to show category and confidence on the image.*
> - *Optimized some UI.*



> *Changelog — 2026-02-01 (v3.9.6)*  
>  
> - *Changed double-click to single-click for showing object class and color.*
> - *Added class info display to show category and confidence on the image.*


> *Changelog — 2026-01-30 (v3.9.5)*  
>  
> - *Fixed opening recent projects issue on Windows/Linux systems.*

> *Changelog — 2026-01-18 (v3.9.5)*  
>  
> - *Supported changing the default save format.*  
> - *Fixed an issue in exporting shapefiles.*  
> - *Optimized the display of the class dropdown list.*  


> *Changelog — 2026-01-16 (v3.9.5)*  
>  
> - *Supported opening recent projects*  
> - *Added annotation statistics and quality check functions*  
> - *Added image annotation matching function*  
> - *Added more image enhancement methods*  
> - *Added a light green theme*  



> *Changelog — 2026-01-13 (v3.9.3)*  
>  
> - *Added polyline support*  
> - *Supported saving multiple custom path configurations*  
> - *Optimized the right-click menu*  
> - *Added the get image information feature*  
> - *Optimized class color settings*  


> *Changelog — 2026-01-06 (v3.9.2)*  
>  
> - *Added YOLO OBB confidence display feature*  
> - *Optimized scan label class functionality*  
> - *Optimized other details*  


> *Changelog — 2026-01-05 (v3.9.1)*  
>  
> - *Fixed GDAL import issues on macOS and Linux*  
> - *Added YOLO-format OBB support*  
> - *Optimized sub-image extraction and format conversion*  
> - *Added DOTA-format export support*  


> *Changelog — 2025-12-29 (v3.9.0)*  
>  
> - *Added macOS version support*  
> - *Improved and optimized UI/UX*  
> - *Enabled right-click quick edit for drawing width, point radius, hollow circle, etc.*  
> - *Optimized format conversion strategy (scanned only files with labels and related data)*  
> - *Optimized color editing strategy (saved category–color mappings directly)*  
> - *Confidence filtering: Applied to YOLO-format points or bounding boxes. For the output results, if a confidence score was appended as the last column, you could choose to filter what was displayed based on the confidence score.*  
>  
> If macOS blocked the app because it was from an unidentified developer:  
>  
> 1. Open **System Settings** → **Privacy & Security**  
> 2. Scroll to **Security**  
> 3. Find the message like: “`<AppName>` was blocked from use because it was not from an identified developer.”  
> 4. Click **Open Anyway**  
> 5. Confirm again in the popup by clicking **Open**  
> 6. We guaranteed the security of the software, but at the moment we couldn’t obtain Apple certification because it required an expensive fee.  


> *Changelog — 2025-11-23 (v3.8.1)*  
>  
> - *Optimized COCO-format data loading*  
> - *Added box zooming functionality*  
> - *Improved Ctrl+Z undo behavior*  
> - *Optimized button bar visuals*  
> - *Added multi-select functionality*  
> - *Optimized point selection*  


> *Changelog — 2025-11-18*  
>  
> - *Fixed GDAL issues*  
> - *Restored small file sizes*  


> *Changelog — 2025-11-17*  
>  
> - *Automatically recorded language and theme settings*  
> - *Other minor optimizations*  


> *Changelog — 2025-09-03*  
>  
> - *Modified mouse wheel zoom behavior: Mouse wheel directly zooms, Ctrl + mouse wheel changes to fine zoom*  



> *Changelog — 2025-08-25*  
>  
> - *Fixed misalignment issue when auto-saving during rapid image switching*  
> - *Added new category reminder in draw mode*  


> *Changelog — 2025-08-22*  
>  
> - *Added import and export functionality for color settings*  
> - *Fixed conflicts between default format and existing format*  


> *Changelog — 2025-08-22*  
>  
> - *Added import and export functionality for color settings*  
> - *Fixed conflicts between default format and existing format*  



> *Changelog — 2025-08-20*  
>  
> - *Added focus mode to hide other targets*  
> - *Enabled loading of previously recorded paths with direct jump to saved image index*  
> - *Added target copy & paste functionality*  
> - *Made polygon vertex circle size adjustable*  

> *Changelog — 2025-08-19*  
>  
> - *Fixed delay when switching images*  
> - *Improved experience when dragging HBB/OBB targets*  
> - *Added Chinese language support*  
> - *Optimized new class creation*


<img width="1916" height="1005" alt="003" src="https://github.com/user-attachments/assets/f06aa7ee-bbf2-4830-8aa0-9242a6b0cb02" />


<img width="1486" height="779" alt="005" src="https://github.com/user-attachments/assets/6f22ced5-2b61-45df-8373-27c98f08c19a" />




## 🚀 Core Features

### 📐 Multiple Annotation Modes
- Supports **HBB** (Horizontal Bounding Box), **OBB** (Oriented Bounding Box), **center points**, and **Polygons**.
- Export formats: **COCO**, **VOC**, **YOLO**, **Mask**, **Esri Shapefile**.

### 🌍 Remote Sensing Data Support
- Supports **multi-band GeoTIFF** and other geospatial formats.
- Customizable band combination display (RGB, NIR, SWIR, etc.).
- Preserves **coordinate system** and georeferenced annotations.

### 🎯 Sub-image Extraction
- Crop arbitrary-sized sub-images with **auto-adjusted annotations**.
- Maintain geospatial coordinates for remote sensing image extractions.

### ⚡ Quick Path Logging
- Press **Enter** to log questionable image paths for secondary review.

### 👁️ One-Click Display
- Toggle annotations on/off instantly for clearer viewing in dense areas.

### 🔍 OBB Rotation Annotation
- Arbitrary-angle OBBs for remote sensing, text detection, etc.
- **Left mouse**: adjust dimensions. **Right mouse**: control rotation.

---

## 📚 Operation Guide

### 📁 File Management
- **Ctrl+S** – Save annotations  
- **Ctrl+R** – Refresh annotations  
- **Clear Configuration** – Reset all settings

---

### 🛰️ Remote Sensing Image Support
**Formats:** `.tif/.tiff`, `.hdr`, `.nc`, `.jpg`, `.png`, `.bmp`  
**Features:**
- Auto channel selection dialog for multi-band images
- Custom band combinations
- Auto coordinate system detection
- Geospatial metadata preservation

---
### Button
-  🔲 Box Selection (M): Draw a box to select multiple targets, right-click to cancel selection. When multiple items are selected, you can drag and delete them.
- 🔍 Zoom to Region (Z): Draw a box on canvas to zoom to that region
-  🎯 Focus (V): Show only selected annotation
-  👁️ Toggle Annotations (H): Show/Hide all annotations
-  🖼️ Fit to View (I): Fit image to window size
---
### 🖼️ Image Navigation
- **← / →**: Previous / Next image  
- **Enter**: Jump to image number  
- **Scroll / Shift+Scroll**: Pan vertically / horizontally  
- **Left-drag empty space**: Move image

---

### 🔍 Zoom & View
- **↑ / ↓** or **Ctrl+Scroll**: Zoom  
- **Ctrl+0**: Reset zoom  
- **Ctrl+F**: Fit to window  
- **Ctrl+H**: Show/Hide annotations

---

### ✏️ Annotation Creation
- **Q**: Toggle draw mode  
- **Point**: Click once  
- **HBB**: Click start → Click end  
- **OBB**: Click corner → Click width → Click height  
- **Polygon**: Click vertices → Double-click to finish

---

### 🔧 Annotation Editing
- Select: **Left/Right click** on annotation  
- Move: **Drag center**  
- Resize HBB/OBB: **Drag corners**  
- Rotate OBB: **Right-drag corner**  
- Delete: **Delete** key

---

### 🎛️ Quick Settings
- **1-5**: Set class  
- **Ctrl+1-5**: Set color  
- **B**: Toggle step size

---

### 🎯 Special Features
- **P**: Sub-image mode  
- **W/A/S/D**: Move canvas  
- **R/F**: Increase/Decrease OBB width  
- **T/G**: Increase/Decrease OBB height  

---

## 💾 Auto Save & Format Conversion

### Auto Save
- Automatic save on image switch/jump
- Manual save with **Ctrl+S**
- Format-specific auto saves:
  - YOLO (Point/HBB)
  - Special OBB format
  - JSON (Polygon)

### Format Conversion
- Convert to **COCO**, **VOC**, **YOLO**, **Mask**, **Shapefile**
- Class mapping support  
- Multiple annotation types in one conversion  
- Mask pixel values configurable

---

## 🗺️ Shapefile Export
- Supports Points, Polygons, Rectangles
- Auto coordinate detection
- Output: `.shp`, `.shx`, `.dbf`, `.prj`
- Attribute and category preservation

---

## 💡 Usage Tips
1. Use **Ctrl+Scroll** for precise zoom  
2. **Q** to toggle draw mode quickly  
3. Use shortcuts for category/color changes  
4. Delete wrong annotations instantly  
5. Always save work (manual or auto)

---

## 🛠️ Remote Sensing Workflow
1. Load georeferenced images  
2. Select band combination (RGB, false color, custom)  
3. Annotate with preserved coordinates  
4. Export shapefile for GIS analysis

---

## ⚠️ Important Notes
- Polygon needs at least **3 points**  
- Always ensure source image has geospatial metadata for shapefile export  

---

## 📋 Annotation Types
- **Point** – center point detection  
- **HBB** – Horizontal bounding box  
- **OBB** – Rotated bounding box  
- **Polygon** – Segmentation tasks  

---

## 📜 License
[MIT License](LICENSE)

---

