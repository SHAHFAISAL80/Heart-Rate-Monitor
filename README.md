# Heart-Rate-Monitor
monitoring heart rate in real-time using a webcam.This is based on an algorithm called Eulerian Video Magnification which makes it possible to see the colours of the face change as blood rushes in and out of the head. It is able to detect the pulses and calculates the heart rate in beats per minute (BPM).This method performs well in real-time.
STEPS

Input: Webcam video feed as the input for heart rate measurement.

Preprocessing: Use MediaPipe (CVZone) to detect and localize the face region in the video frames.

Spatial Decomposition: Decompose the video frames into multiple spatial frequency bands using a pyramid-based approach.

Temporal Filtering: Apply band-pass filtering techniques to isolate the desired frequency range associated with the heartbeat.

Magnification: Amplify the subtle temporal variations related to the heartbeat for better visibility.

Measurement: Extract the amplified signal and estimate the heart rate in beats per minute (bpm) using appropriate signal processing techniques.

Visualize Results: Use CVZone LivePlot to visualize the heart rate estimation results.

                                       ┌───────────────────┐
                                       │       Input       │
                                       │   Webcam Video    │
                                       └───────────────────┘
                                                │
                                                v
                                       ┌───────────────────┐
                                       │   Preprocessing   │
                                       │   Face Region     │
                                       │    Detection      │
                                       └───────────────────┘
                                                │
                                                v
                                       ┌───────────────────┐
                                       │    Spatial        │
                                       │  Decomposition    │
                                       └───────────────────┘
                                                │
                                                v
                                       ┌───────────────────┐
                                       │    Temporal       │
                                       │   Filtering       │
                                       └───────────────────┘
                                                │
                                                v
                                       ┌───────────────────┐
                                       │   Magnification   │
                                       └───────────────────┘
                                                │
                                                v
                                       ┌───────────────────┐
                                       │    Measurement    │
                                       │   Heart Rate      │
                                       │   Estimation      │
                                       └───────────────────┘
                                                │
                                                v
                                       ┌───────────────────┐
                                       │    Visualize      │
                                       │    Results        │
                                       │   CVZone LivePlot │
                                       └───────────────────┘
