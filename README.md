#@title Install Library
import os, sys
from google.colab import drive
drive.mount('/content/drive',force_remount=True)
nb_path = '/content/notebooks'
os.symlink('/content/drive/My Drive/Colab Notebooks/mylib', nb_path)
sys.path.insert(0,nb_path)

!pip install --target=$nb_path qrcode
!pip install --target=$nb_path selenium
!pip install --target=$nb_path opencv-python
!pip install --target=$nb_path matplotlib
