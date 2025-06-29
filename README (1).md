# 🧢 Hat Classifier Project

This project focuses on analyzing and classifying images of hats using basic computer vision techniques and exploratory data analysis. It loads a dataset of hat images, performs preprocessing, visualizes patterns using cross-correlation, and examines class-wise distributions.

---

## 📂 Project Structure

```
Hat Classifier Project.ipynb
├── Google Drive Mount
├── Dataset Extraction (.zip)
├── Image Preprocessing
├── Cross-Correlation Analysis
├── Statistical Visualization
```

---

## 📊 Features

- ✅ Load dataset from Google Drive and extract
- ✅ Convert hat images to grayscale and resize to 128x128
- ✅ Normalize pixel values
- ✅ Visualize cross-correlation between images
- ✅ Boxplots of average pixel intensity per class

---

## 📁 Dataset

- Format: `.jpg` images
- Location: Mounted Google Drive
- Structure: 
  ```
  AI Dataset/
    ├── HatType1/
    ├── HatType2/
    └── HatType3/
  ```

Each subfolder contains images of a specific hat type (class label).

---

## ⚙️ Requirements

- Python 3.7+
- Jupyter Notebook
- Google Colab (for Drive integration)

### Python Libraries Used

```bash
opencv-python
matplotlib
numpy
seaborn
scikit-learn
```

---

## 🚀 How to Run

1. Open `Hat Classifier Project.ipynb` in Google Colab.
2. Upload your dataset ZIP file to Google Drive.
3. Update the ZIP path in the notebook:
   ```python
   zip_path = "/content/drive/MyDrive/AI Dataset.zip"
   ```
4. Run all cells to extract, preprocess, and analyze images.

---

## 🧠 Methodology

- **Preprocessing:**
  - Convert to grayscale
  - Resize to 128x128
  - Normalize pixel values to [0, 1]

- **Cross-Correlation:**
  - Compute pixel-wise correlation between 20 sample images
  - Visualize similarity matrix as a heatmap

- **Boxplot:**
  - Mean pixel intensity computed per image
  - Boxplots show class-wise variance

---

## 📈 Results

- The heatmap reveals how similar images are across and within classes.
- Boxplots help identify which classes have more visual intensity variance.

---

## 🔍 Limitations

- Only grayscale data is used (color may be informative).
- No actual model is trained — it’s a preprocessing and visualization analysis.
- Works with small subsets of data for visualization (e.g., 20 images for correlation).

---

## 📌 Future Improvements

- Train an actual classifier (e.g., CNN or SVM).
- Use data augmentation for model generalization.
- Visualize class separability using PCA or t-SNE.
- Automate Drive mounting & dataset download.

---

## 📜 License

This project is open-source and free to use for educational purposes.

---

## 🙋‍♂️ Author

Made with ❤️ by Tanveer Hassan  
