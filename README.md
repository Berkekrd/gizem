## 1. `kaggle.json` Dosyasını Google Colab'a Yükleyin

Google Colab'da aşağıdaki adımları izleyerek `kaggle.json` dosyasını yükleyin:

```python
from google.colab import files
files.upload()
```

## 2. Veri Seti Bağlantısı

Bu kod bloğu sayesinde kaggle ile bağlantı sağlanıcak ve otomatik bir şekilde veri seti indirilicektir.

```python
!pip install kaggle
import os
os.environ['KAGGLE_CONFIG_DIR'] = '/content/.kaggle'
!kaggle datasets download -d masoudnickparvar/brain-tumor-mri-dataset
!unzip brain-tumor-mri-dataset.zip
```
