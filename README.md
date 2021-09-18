AI Trainer For Gym

Many people who being exercising lack professional guidance. They tend to miss out on a lot of potential gains either by performing the exercise incorrectly
or by having poor posture while doing it. In some cases they may even end up doing more harm than good.

Our aims to help in that regard by helping and guiding when performing a variety of exercises.

Currently Supported Exercise Analysis:-

- Squat: exaggerated knees-forward checking
- Dumbbell Shoulder Press: exaggerated arm bend and extension checking
- Bicep Curls: horizontal elbow deviation from shoulder checking

Future Changes:-
1. Multiple Pose Estimations for One User

Current: The model estimates joints for all subjects found in the input image; we then analyze the output and extract the pose that is most likely to be the user.

Possible Improvements:

(a) Modify model and training data to only estimate a single 'best' pose.

or

(b) Implement re-identification and support multiple users at once. This is viable as forward propagation time does not increase with multiple poses being estimated.

2. Webcam Image Data Transfer:-

Current: Webcam captures are encoded in base64 strings and a post request is sent to the server with the data (note: this was done for ease of implementation
due to the hackathon time constraint).

Possible Improvements: Implement web sockets to transfer webcam captures instead.
