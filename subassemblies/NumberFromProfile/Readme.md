# Number from profile

Experimental subassembly.

## Usage

Do you want to set parameters graphically with profile? Now you can, just target the subassembly to a profile and use multiplier to edit the targeted elevation into desired number.

### Example

### Superelevation by profile

Just target the subassembly to desired profile and reference its output to other subassemblies. You can create a "superelevation" definition with profiles close to height zero. For example height = 3 m will be then multiplied by 0.01 and the output will be 3% . Like superelevation.

It would be more convenient than using supperelevation graph which can be tricky to edit.

### Height of a curb

You can specify a curb height with the subassembly no matter how high real road profile is.

### Other ...

Or you can set up width of a pavements with profile... use your imagination.

## Parameters

| Name              | Type   | Description                                                                                                                                         |
| ----------------- | ------ | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| Output for layout | double | Temporary number when creating asssembly. The number will be overwritten with target elevation if valid. But it will be used if no target is valid. |
| Multiplier        | double | Compose the result by using this parameter. Target elevation multiplied by this param is your result.                                               |
| Result            | double | OUTPUT parameter to be referenced into other subassemblies.                                                                                         |

## Codes

### Points

\_LayoutOnly will be applied only in assembly creation. The code for showing the subassembly is switch off when building corridor.

### Lines

none

### Shapes

none

## Versions

| Version    | Date       | Description   |
| ---------- | ---------- | ------------- |
| 2020 1.0.0 | 2024-09-22 | First release |
|            |            |               |
