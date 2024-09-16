# Layer

A generic subassembly allows you to create a layer for anything. Layer can be a road layer - asphalt, concrete, gravel...

## Usage

### Widths

1. Create classic road structure. Connect more layers into one big assembly.

Schema

- |------
- |--------
- |-----------

2. Create a reconstruction road structure

- "xxx" is a current road structure that remains still
- "---" is a new road structure - see that layers widths differ

Schema

- |----------
- |xxx-------
- |xxxxxx----

3. Create an inverse reconstruction road structure

- "xxx" is a current road structure that remains still
- "---" is a new road structure - see that layers widths differ

Schema

- |----------
- |-------xxx
- |----xxxxxx

### Slopes

Reconstruction can be tricky and you will need to dynamicaly change the slope of a subassembly.

- Superelevation = use generic subassembly LinkWidthSlope to read specific superelevation and reference it to Layer subassembly
- Targeting - offset and elevation can change slope

## Targets

| Name      | Type      | Description                                 |
| --------- | --------- | ------------------------------------------- |
| Offset    | offset    | Changing width - BUT MARKED POINT beats it! |
| Elevation | elevation | Changing slope - BUT MARKED POINT beats it! |

## Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
|      |      |             |

## MARKED POINTS

Marked points allows you to connect for the width of previous subassemblies.

### Example

You are creating 3 layered road construction. Number 1,2,3 define marked points. Let´s assume you use dynamic targeting for defining width of layer 1. You cannot define the exact width for 2 and 3. You use MARKED POINTS to specify the width.

- ---1
- ---|---2
- -------|---3

There are 4 MARKED POINTS generated dynamically according to CODE ID parameter

- P1 ----- P2
- | ------- |
- P3 ----- P4

CodeID = FL (first layer) and Marked Points generated

- P1 = FLMPINTOP = FirstLayerMarkedPointINsideTOP
- P2 = FLMPOUTTOP
- P3 = FLMPINBOTTOM
- P4 = FLMPOUTBOTTOM

## Codes

Codes are generated dynamically based on the Code ID parameter.

- Code ID: "FL"

### Points

based on the inputs codes can be for example

- FLPointTopOut
- FLPointBottomOut
- FLPointBottomIn
- FLPointTopIn

### Lines

- FLLineTop
- FLLineOut
- FLLineBottom
- FLLineIn

### Shapes

- FLShape

## Versions

| Version    | Date       | Description   |
| ---------- | ---------- | ------------- |
| 2020 1.0.0 | 2024-09-14 | First release |
|            |            |               |
