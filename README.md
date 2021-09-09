# DocumentScanner_OpenCV
## created a Document Scanner using OpenCV library
## Tools used : `OpenCV`, `Numpy`, `imutils`

#### Description:

A simple mobile document scanner has been implemented using OpenCV library. It consists of mainly three steps as follows
- Firstly, read the image and convert it into grayscale. Then find the edges using Canny Edge Detector
- FInd out the countours in the edged image. Here Countours are nothing but the points along the boundary of an object. As the document is mainly focussed, we need the largest countours. So that we can get rid of small countours.
- Apply four point transform using [`transform.py`](https://github.com/raghu826/DocumentScanner_OpenCV/blob/main/transform.py) to obtain the top-down view of the contoured image. To get the black and white effect, image is converted to grayscale and threshold it to get the scanned document.

## To run the code `python scan.py --image images/imageName.jpg`



























