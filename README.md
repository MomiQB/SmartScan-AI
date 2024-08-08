# SmartScan-AI

_Authors_: Simone Vaccari, Alessio De Luca, Davide Vettore

**SmartScan AI** is an advanced machine learning tool capable of identifying lumps and categorizing them as either cancerous or non-cancerous.  \
Our primary **goal** is to provide oncologists with an exceptionally precise tool to fasten and enhance diagnoses, both crucial elements for improved early detection.

> Breast cancer is a type of cancer that starts in the cells of the breast. It can occur in both men and women, but it's much more common in women.  \
> Breast cancer can begin in different parts of the breast, such as the ducts or the lobules. It can spread to other parts of the body through the lymphatic system or bloodstream.  \
> Early detection through screening and awareness campaigns is crucial for successful treatment.

Starting from a dataset of Breast Ultrasounds and their masks, we extract radiomic features and create a robust **classifier** that is able to distinguish between benign and malignant regions. Subsequently, we design and train a **U-Net** that is able to automatically detect the regions of interest. Finally, we design a **dashboard** with an intuitive interface for diagnostics.  

### _Content_:
Main directory:
- [Health_Class.ipynb](https://github.com/MomiQB/SmartScan-AI/blob/main/Health_Class.ipynb): notebook for the training of the classifier. Different models are tested: SVM, Random Forest, MLP.
- [Health_Segm.ipynb](https://github.com/MomiQB/SmartScan-AI/blob/main/Health_Segm.ipynb): notebook for the training of the segmentation model.
  
_streamlit-dashboard_ directory:
- [login.py](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/login.py): login interface for the dashboard
- [credentials.yaml](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/credentials.yaml): file to store the credentials of the registered users
- [functions.py](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/functions.py): utility functions for the dashboard
- [style.css](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/style.css): CSS file with styling for the dashboard
- [requirements.txt](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/requirements.txt): packages versions to make the app work
- [pages/main](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/pages/main.py): main file for dashboard
- [pages/normalization_all.csv](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/pages/normalization_all.csv): csv file with information for feature normalization
- [pages/register.py](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/pages/register.py): registration interface
- [pages/svm_final.joblib](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/pages/svm_final.joblib): best trained classifier
- [pages/segmUnet100_aug.keras](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/pages/segmUnet100_aug.keras): best trained U-Net model
- [pages/logo_smartscan_nobg.png](https://github.com/MomiQB/SmartScan-AI/blob/main/streamlit-dashboard/pages/logo_smartscan_nobg.png): logo image





