#1. python3
conda create --name=labelme python=3.6
conda activate labelme
# conda install -c conda-forge pyside2
# conda install pyqt
# pip install pyqt5  # pyqt5 can be installed via pip on python3
pip install labelme==3.16
pip install numpy==1.16
# or you can install everything by conda command
# conda install labelme -c conda-forge

# 2.Type labelme and window will pop up and create your pixel annotation using
labelme and store it into json format

# 3. cd detectronn2session where our labelme2coco.py is present 
# then type ==> python labelme2coco.py label_mask --output final_dlcvnlp.json
# here labelme2coco.py is same as we convert our files from xml to csv
# label_mask is the folder from where we are picking our json files
# final_dlcvnlp.json is the final conversion we want.
# but i have used the tranival.json in data folder.

# 4. open the detectron2 file in colab.