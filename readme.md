<h2>How to run?</h2>

<h3>Install necessary modules:</h3>
  
  pip install --upgrade imutils
  <h2>One of these should works:</h2>
  conda install -c conda-forge opencv=4.1.0
  conda install -c conda-forge imutils
  conda install -c menpo opencv3

  pip install opencv-python <br>
  pip install opencv-contrib-python or pip install opencv-contrib-python --user

  <h2>The error you could faced:</h2> "The function is not implemented. Rebuild the library with Windows, GTK+ 2.x or Cocoa support" - 
cv2.error: OpenCV(4.1.1) ...\...\..path: error: (-2:Unspecified error) The function is not implemented. 
Rebuild the library with Windows, GTK+ 2.x or Cocoa support. If you are on Ubuntu or Debian, 
install libgtk2.0-dev and pkg-config, then re-run cmake or configure script in function 'cvShowImage'

  <h3>Solution:</h3>
pip install opencv-contrib-python 

  <h3>Run: </h3>
python main.py --i images/test-img1.jpg  --east frozen_east_text_detection.pb

<h3>At several cases you should delete modules:</h3>
  conda remove opencv
  conda activate base
  pip uninstall opencv-python

