# Custom Tarot Spread Builder

An interactive, single-file web application for creating, visualizing, and exporting custom tarot card spreads. This tool is designed for tarot enthusiasts and readers who want a digital canvas to design and interpret their readings.

**Original Author:** 星罗工作室 (XingLuo Studio)

**Note:** The user interface of the application is in Chinese.

---

## ✨ Features

This application runs entirely in your web browser, requiring no backend or internet connection after loading. All user data, such as custom card images and spread templates, is stored locally on your machine using IndexedDB and LocalStorage.

### 🎨 Dynamic Spread Canvas
* **Interactive Workspace:** A large, pannable, and zoomable canvas to build your spreads.
* **Drag & Drop:** Easily add and arrange position markers and tarot cards.
* **Element Control:** Select, move, and delete elements with mouse or keyboard shortcuts.
* **Reset View:** Automatically zoom and pan to fit all placed elements perfectly in the viewport.

### 🃏 Card and Position Management
* **Position Markers:** Add numbered markers with custom text to define the meaning of each position in the spread (e.g., "1: The Past," "2: The Present").
* **Full 78-Card Deck:** Select and place any card from the Major and Minor Arcana.
* **Card Orientation:** Place cards upright or reversed, and apply custom rotation angles.

### 🖼️ Deck Customization
* **Custom Card Images:** Replace the default card faces with your own imagery. Click "上传图片" (Upload Image) on any card in the "牌面信息" (Card Information) tab.
* **Image Processing Tools:**
    * **Fit to Card:** Resizes your image to fit within the card's boundaries, preserving the full picture.
    * **Fill Card (Crop):** Use an intuitive cropper to select the exact portion of your image to fill the card face.
* **Batch Upload:** Quickly customize your entire deck by naming your image files according to the card's ID (e.g., `0.png` for The Fool, `22.jpg` for the Ace of Wands) and using the "批量上传牌面" (Batch Upload Faces) button.
* **Data Persistence:** Your custom images are saved in the browser's IndexedDB, so your personalized deck is always available.

### 💾 Save, Load, and Export
* **Export as Image:** Generate a high-quality PNG image of your completed spread, perfect for sharing or archiving.
* **Copy as Image:** Copy the spread directly to your clipboard to easily paste into other applications.
* **Save as JSON:** Save the entire spread layout (including all card and position data) as a `.json` file. This allows you to save your work and continue later.
* **Import from JSON:** Load a previously saved `.json` file to restore a spread on the canvas.

### 📂 Spread Templates
* **Built-in Templates:** Comes pre-loaded with common spreads like the *Three Card Spread*, *Celtic Cross*, and *Horseshoe Spread*.
* **Save Custom Templates:** Design your own spread layout with position markers and save it as a custom template for future use.
* **Manage Templates:** Your custom templates can be easily accessed, applied, or deleted.

### ⚙️ Data Management
* **Clear Custom Images:** Remove a single custom card image or all of them at once.
* **Factory Reset:** A dedicated button to clear all user data (custom images and saved templates) from the browser, restoring the application to its original state.

## 🚀 How to Use

### Live Demo
You can host this `V1.5.html` file on a service like GitHub Pages for easy access.

### Local Usage
1.  Download the `塔罗牌阵自定义推演器 V1.5.html` file.
2.  Open the file in any modern web browser (e.g., Google Chrome, Mozilla Firefox, Microsoft Edge).
3.  All features are self-contained and will work offline.

## 🛠️ Technologies Used

* **Frontend:** HTML5, CSS3, Vanilla JavaScript
* **Libraries:**
    * `html2canvas.js`: For exporting the spread canvas to a PNG image.
    * `cropper.js`: For the interactive image cropping functionality.
* **Browser APIs:**
    * `IndexedDB`: For storing custom card image data.
    * `LocalStorage`: For storing custom spread templates.
    * `File API`: For importing/exporting JSON files.
    * `Clipboard API`: For the "Copy as Image" feature.

## 📄 License

This project is open-source and available under the [MIT License](https://opensource.org/licenses/MIT).
