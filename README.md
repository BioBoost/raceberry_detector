# Raceberry Detector

Detect the Pololu robots in a 3D maze using this implementation in AVS. Actual coordinates and direction are communicated to server in a JSON string of following format:

```json
{"robot3": {"x": 1142.264, "y": 576.689, "angle": 1.540 },"robot2": {"x": 1200.844, "y": 705.500, "angle": 0.846 }}
```

x and y are the location of the robots in the interval [0..1]. The angle is expressed in radians.

## Camera setup

Using AV Manta G504-C with an 8mm lens.

Exposure is set to 40'000 and Pixel Format is BayerRG8.


## Test with netcat

Just setup netcat TCP server on linux using following command:

```shell
netcat -lk 1337
```