# Raceberry Detector

Detect the Pololu robots in a 3D maze using this implementation in AVS. Actual coordinates and direction are communicated to server in a JSON string of following format:

```json
[{ "id": "robot_1", "x": 0.125, "y": 0.987, "a": 128 },{ "id": "robot_2", "x": 0.455, "y": 0.012, "a": 12 }]
```

x and y are the location of the robots in the interval [0..1]. The angle (a) is expressed in degrees.