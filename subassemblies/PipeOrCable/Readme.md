# Pipe or cable

The subassembly allows you to create cable object or a pipe object depending on the "wall thickness" parameter.

## Usage

Want to create a 3D solid of a cable or a pipe? Just create an alignment with profile or 3D feature line and apply the subassembly for a corridor.

Why should I use corridor for cable creation? Well, you can benefit from corridor regions to specify where the cable should be protected with a pipe ...

## Parameters

| Name               | Type   | Description                                                                                                               |
| ------------------ | ------ | ------------------------------------------------------------------------------------------------------------------------- |
| Alignment position | List   | Where is your 3D path located? On top of the pipe? On the bottom? Or you are modeling cable with center position 3D path? |
| Wall thickness     | Double | Input 0 in case of cable                                                                                                  |
| Diameter           | Double | Diameter = 2x wall thickness + empty space of the pipe.                                                                   |
| Code ID            | String | Codes for the subassembly are generated dynamically. See Codes section                                                    |

## Codes

Codes are generated dynamically based on the Code ID parameter.

- Code ID: "EL"
- Wall thickness: 0

### Points

based on the inputs codes can be for example

- ELCableTop
- ELCableBottom
- ELCableRight
- ELCableLeft
- ELCableCenter

### Lines

- ELCableLineTop
- ELCableLineBottom

### Shapes

- ElCableShapeWall
- ELCableShapeEmpty - empty space of a pipe
- ELCableShapeVolume - union of Wall + Empty space

## Versions

| Version    | Date       | Description   |
| ---------- | ---------- | ------------- |
| 2020 1.0.0 | 2024-09-14 | First release |
|            |            |               |
