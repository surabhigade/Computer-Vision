# Computer-Vision : DoctorStrange Sheild Effect

check out the Output for this project below.

![drstrange](https://github.com/user-attachments/assets/668fe909-db66-46f1-b1e3-4cf7ddda857c)

# Hand Tracking with Overlay Video Effect

 ## Overview
 
This Python program uses a webcam to track hand movements and overlays a video clip (a shield image) when two hands come close together. It creates a shield effect that responds to hand gestures.
 
## Features

- **Real-time Hand Tracking:** Detects hands using the webcam.
- **Interactive Overlay:** Displays a video clip when two hands are close.
- **Dynamic Scaling:** Adjusts the overlay size based on hand size.
- **Video Output:** Saves the processed video as an .mp4 file.

## Dependencies

- **OpenCV:** For video capture and processing.
- **cvzone:** For hand detection.
 - **math:** For calculating distances.

Install the dependencies with:

```bash
 pip install opencv-python cvzone
```

 ## How It Works

1. **Hand Detection:** Captures video and detects hands in each frame.
 2. **Distance Calculation:** Measures distance between two hands and triggers the shield effect if the distance is below a threshold.
3. **Overlaying Video:** Adds the shield video at the hand position, scaling it based on hand size.
4. **Saving Video:** Saves the final video as `output.mp4`.

## Usage

### Running the Program

1. Ensure the webcam is connected.
2. Place `shield.mp4` in the script directory.
3. Run the script:

```bash
python hand_tracking_shield.py
```
4. The webcam feed will open. Bring your hands close together to see the shield effect.
5. Press `q` to exit the program.

### Customizing

- **Threshold Distance:** Adjust the `distance` variable to change when the shield appears.
- **Overlay Scaling:** Modify the `mapFromTo` function to change the scaling of the shield.

### Output

- The video is saved as `output.mp4`.
- The live video feed is displayed with the overlay applied.

## Troubleshooting

- **Webcam Issues:** Check webcam connection if the video stream doesn't open.
- **Shield Video Problems:** Ensure `shield.mp4` is correctly formatted and located.
  

## Author
**Surabhi Gade**  

Developed for a computer vision project with interactive hand tracking and video overlays.
 
## Acknowledgments

Thanks to the creators of `cvzone` for the hand detection library.
