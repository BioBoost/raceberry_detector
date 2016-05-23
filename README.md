# Raceberry Detector

Detect the Pololu robots in a 3D maze using this implementation in AVS. Actual coordinates and direction are communicated to server in a JSON string of following format:

```json
[{"id": "robot3", "state": {"x": 2104, "y": 72, "angle": 4.230 }},{"id": "robot6", "state": {"x": 1131, "y": 79, "angle": 1.346 }},{"id": "robot7", "state": {"x": 2275, "y": 525, "angle": 1.023 }},{"id": "robot1", "state": {"x": 706, "y": 716, "angle": 5.524 }},{"id": "robot4", "state": {"x": 1871, "y": 727, "angle": 2.721 }},{"id": "robot2", "state": {"x": 1310, "y": 842, "angle": 1.967 }}]
```

x and y are the location of the robots in millimeters. The angle is expressed in radians.

## Camera setup

Using AV Manta G504-C with an 8mm lens.

Exposure is set to 40'000 and Pixel Format is BayerRG8.


## Test with netcat

Just setup netcat TCP server on linux using following command:

```shell
netcat -lk 1337
```