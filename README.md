# unique-faces-count-in-video
python code to identify unique number of faces in a video and output the video with a visible real time counter

# Libraries used for for face capturing and reorganization:
1. cv2
2. face_recognition

# Steps Undertaken:
1. importing necessary libraries
2. creating instances for input and output videos.
3. Initializing variables to store unique faces encoding and faces encodig in a frame and face count counter
4. Iterating video frame by frame(Image)
  4A. Convert the image from BGR color (which OpenCV uses) to RGB color (which face_recognition uses)
4B. Find all the faces and face encodings in the current frame of video
4C. See if the face is a match for the known face(s)
4C(i). for first frame save faces in known faces and increase counter
4C(ii) if faces already identified then do not count it else save in known faces list and increase counter
4D. update and display count on frame
4E. write each frame to output video

Input video: faces.mp4
Output video : output_faces_final_more restricted.avi (more restricted version detect 32 unique faces)

Note: model can be refined more for  accurate results as it is just a rough implementation 
