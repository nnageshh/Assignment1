# Assignment1A - Horizontal Edge Detector code

# to do the mathematical caluclations
import numpy as np
import cv2
# to extract the information from the url
from urllib.request import urlopen

# to read the image from url and coverted to array format
def url_to_image(url):
  resp=urlopen(url)
  image=np.asarray(bytearray(resp.read()),dtype="uint8")
  image=cv2.imdecode(image,cv2.IMREAD_COLOR)
  return image
  
# passing the image from the url and storing into image variable
image=url_to_image("https://fontsarena-cd5e.kxcdn.com/wp-content/uploads/2019/04/helvetica-now-font-400x364.png")

# importing library to display the image
from google.colab.patches import cv2_imshow
cv2_imshow(image)

# passing the area of the canvas (width & height)
edges=cv2.Canny(image,100,200)

#disyplaying the edges of the letters in word
cv2_imshow(edges)

# code for idetifying the horizontal edges of the characters in the image

kernel=np.float32([[-1,-1,-1],[0,0,0],[1,1,1]])
dist=cv2.filter2D(image,-1,kernel)
cv2_imshow(dist)
