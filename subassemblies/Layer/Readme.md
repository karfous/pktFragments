# Layer

A generic subassembly allows you to create a layer for anything. Layer can be a road layer - asphalt, concrete, gravel...

## Usage

How to use this subassembly? Well, there are quite a few possible ways...

### Classic road structure

Create classic road structure. Connect more layers into one big assembly.

Imagine that | is you axis. And dashes "-" shows width of each layer. The picture below consist of three layers. You can define extra width for base layers for example :)

- |------
- |--------
- |-----------

### Create a reconstruction road structure

- "\_\_\_" this is a current road structure that reamins still
- "xxx" is a current road structure that needs to go away
- "---" is a new road structure - see that layers widths differ

Schema

- |xxxxx----------
- |**\_**xxx-------
- |**\_**xxxxxx----

### Create an inverse reconstruction road structure

Very similar to previous example but inverse.

Schema

- |----------xxxx
- |-------xxx\_\_\_\_
- |----xxxxxx\_\_\_\_

## Slopes

Reconstruction can be tricky and you will need to dynamicaly change the slope of a subassembly.

- Superelevation = currently the subassembly cannot read superelevation but use generic subassembly LinkWidthSlope to read specific superelevation and reference it to Layer subassembly
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

You are creating 3 layered road construction. Number 1,2,3 define marked points at the end of each new layer. Let´s assume you use dynamic targeting for the first layer width.

You cannot define the exact width for 2 and 3. Because first layer change its width by targets. You use MARKED POINTS to specify the width instead.

- ---1
- ---|---2
- -------|---3

### How are MARKED POINTS GENERATED ?

There are 4 MARKED POINTS generated dynamically according to CODE ID parameter of each layer.

This schema show marked points for only 1 layer.

- P1 ----- P2
- | |
- P3 ----- P4

First layer can have CodeID = FL (first layer) and Marked Points generated for this layer will have NAMES like

- P1 = FLMPINTOP = FirstLayerMarkedPointINsideTOP
- P2 = FLMPOUTTOP
- P3 = FLMPINBOTTOM
- P4 = FLMPOUTBOTTOM

## Codes

Codes are generated dynamically based on the Code ID parameter. Chnage Code ID according to your needs ...

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
