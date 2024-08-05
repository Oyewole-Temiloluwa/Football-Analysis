#Football Analysis Software
This project involves the development of a football analysis software that detects players on the pitch, calculates the possession of both teams, estimates the speed and distance covered by each player, and more. The software leverages computer vision techniques and deep learning models to analyze football matches and provide detailed statistics.

Features
- Player Detection: Identifies and tracks football players on the pitch using YOLOv5.
- Team Possession: Calculates and displays the possession percentage for both teams.
- Player Speed: Estimates and displays the speed of each player.
- Distance Covered: Calculates the distance covered by each player during the match.
- Camera Movement Estimation: Adjusts for camera movement to maintain accurate tracking.

Project Structure
1. YOLOv5 Model Training
  - football_training_yolo_v5.ipynb: Jupyter notebook for training the YOLOv5 model on football data.
  - yolov5lu.pt: Pre-trained YOLOv5 model weights.
    
2. Player and Ball Detection
  - tracker.py: Main script for tracking players and the ball.
  - player_ball_assigner.py: Assigns detected objects to players and the ball.

3. Team Assignment
  - team_assigner.py: Assigns detected players to their respective teams based on color detection.

4. Speed and Distance Estimation
  - speed_and_distance_estimator.py: Estimates the speed and distance covered by each player.
  - camera_movement_estimator.py: Estimates and adjusts for camera movement.

5. Utility Scripts
  - bbox_utils.py: Utility functions for bounding box operations.
  - video_utils.py: Utility functions for video processing.

6. Color Assignment
  - color_assignement.ipynb: Jupyter notebook for color-based team assignment.
