To run this Python script, ensure that the following packages are installed:

1. numpy
2. opencv-python
3. pip (usually installed by default)
4. dlib

Your IDE might require additional packages or updates. (do them)

During installation, you might encounter errors such as "cannot build wheel" when installing the dlib package using the pip method. This is likely due to compatibility issues between the package's version and Python's version.

If you're using an older version of Python (Python 3.8 or lower), you can try the usual pip method to install dlib. Otherwise, follow these steps:

1. Install Python 3.11.
2. Place the file named "dlib-19.24.1-cp311-cp311-win_amd64.whl" (included with the file) in the folder where you are running the script.
3. In the terminal, execute the following command: 
   ```
   python -m pip install dlib-19.24.1-cp311-cp311-win_amd64.whl
   ```

Ensure that the following files are included within the running folder (these files are provided):
- "shape_predictor_68_face_landmarks.dat"
- "left.wav"
- "right.wav"

To switch the camera to an external input (e.g., a PS3 camera), change the value from 0 to 1 in line 207:
```
cap = cv2.VideoCapture(1)
```

Ensure proper lighting towards your eyes for optimal performance.

You can adjust the frames as needed according to your application to control the responsiveness.

I recommend to use pycharm instead of VS code. make sure to setup venv properly.