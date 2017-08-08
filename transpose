import os
from PIL import Image

rootdir = "C:/caffe-project/Ages/label_image/1_5"
for root, dirs, files in os.walk(rootdir):
    for file in files:
        filename=str(file)
        currentPath = "C:/caffe-project/Ages/label_image/1_5/" + filename
        #print('the fulll name of the file is :' + currentPath)

        image = Image.open(currentPath)
        out = image.transpose(Image.FLIP_LEFT_RIGHT)
        newname = "C:/caffe-project/Ages/label_images/1_5/" + filename[0:23] + "(1).bmp"
        out.save(newname)

print "succeed"
