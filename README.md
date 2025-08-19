# Zeyoo Image Annotation Tool

A powerful and versatile image annotation software designed for both **general computer vision** and **remote sensing** applications.  
Supports **multiple annotation types**, **remote sensing geospatial data**, and **format conversions** for major AI and GIS workflows.

> *Changelog — 2025-08-19*  
>  
> - *Fixed delay when switching images*  
> - *Improved experience when dragging HBB/OBB targets*  
> - *Added Chinese language support*  
> - *Optimized new class creation*



<img width="1916" height="1000" alt="002" src="https://github.com/user-attachments/assets/3ea4a5f8-50cb-4af3-93a7-07d7dbfcc368" />


Download: 

https://ai.zeyuxu.com/zeyoo

https://github.com/zeyu-rs/Zeyoo-Annotation/releases


---
## 🌟 Highlight Tips
1. Double-click to apply the target's color and other properties to the toolbar.  
2. Annotations are saved automatically when switching images. You can also press **Ctrl+S** to save manually.  
3. Supported input/output types (input formats can be auto-detected):  

| Type | Supported Input Formats | Default Output Format | Supported Convertible Output Formats |
|------|------------------------|-----------------------|---------------------------------------|
| Point | YOLO | YOLO | YOLO / Esri Shapefile / Image mask |
| Horizontal Bounding Box | YOLO / VOC / COCO | YOLO | YOLO / VOC / COCO / Esri Shapefile / Image mask |
| Oriented Bounding Box | DOTA | DOTA | DOTA / Esri Shapefile / Image mask |
| Polygon | Labelme JSON / COCO / YOLO | Labelme JSON | COCO / YOLO / Esri Shapefile / Image mask |

> **Note:** Input formats can be auto-detected.


<img width="1916" height="991" alt="005" src="https://github.com/user-attachments/assets/afbf58d4-aec2-458c-835e-e201725233d0" />


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

