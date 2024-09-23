# Number from profile

## Usage

Experimental subassembly. Do you want to set parameters graphically with profile? Now you can, just target the subassembly to a profile and use multiplier to edit the targeted elevation into desired number.

### Example

You can set up superelevation with profile. Just target the subassembly to desired profile and reference its output to other subassemblies. It would be more convenient than using supperelevation graph.

Or you can set up width of a pavements ... use your imagination.

## Parameters

| Name              | Type   | Description                                                                                                                                         |
| ----------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| Output for layout | double | Temporary number when creating asssembly. The number will be overwritten with target elevation if valid. But it will be used if no target is valid. |
| Multiplier        | double | Compose the result by using this parameter. Target elevation multiplied by this param is your result.                                               |
| Result            | double | OUTPUT parameter to be referenced into other subassemblies.                                                                                         |

## Codes

### Points

\_LayoutOnly will be applied only in assembly creation. The code is switch off when building corridor.

### Lines

none

### Shapes

none

## Versions

| Version    | Date       | Description   |
| ---------- | ---------- | ------------- |
| 2020 1.0.0 | 2024-09-22 | First release |
|            |            |               |
