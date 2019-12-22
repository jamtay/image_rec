General overview: https://www.pyimagesearch.com/2018/06/18/face-recognition-with-opencv-python-and-deep-learning/


**To run:**

1. Download opencv: https://www.pyimagesearch.com/2018/09/19/pip-install-opencv/
2. Create virtualenv: `mkvirtualenv cv -p python3`
3. Download dependencies: `workon cv && pip3 install dlib && pip3 install face_recognition && pip3 install imutils`
4. Setup dataset: 4.1) `mkdir dataset` 4.2) `mkidr your_name` 4.3) Add images for labelled 00000000.jpg & 00000001.jpg etc for each image of yourself.  Repeat for other people
5. Encode images:  `python3 encode_faces.py --dataset dataset --encodings encodings.pickle`
6. Run: `python3 recognize_faces_video.py --encodings encodings.pickle --output output/webcam_face_recognition_output.avi --display 1`

**Project structure**

- bin (pip3, python3, wheel etc)
- include (python3.7m folder)
- lib (python3.7 folder (dependencies))
- dataset (subfolders of peoples names, with jpg files labelled 00000000.jpg, 00000001.jpg etc of each person)
