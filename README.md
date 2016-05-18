# Raceberry Detector

Detect the Pololu robots in a 3D maze using this implementation in AVS. Actual coordinates and direction are communicated to server in a JSON string of following format:

```json
{"robot3": {"x": 1143.286, "y": 575.631, "angle": 88.341 },"robot2": {"x": 1201.873, "y": 704.481, "angle": 48.571 }}
```

x and y are the location of the robots in the interval [0..1]. The angle is expressed in radians.

## Camera setup

Using AV Manta G504-C with an 8mm lens.

Exposure is set to 40'000 and Pixel Format is BayerRG8.



robot%0%": {"x": %1%, "y": %2%, "angle": %3% },