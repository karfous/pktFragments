# Yes No switch

Experimental subassembly written in NET. Not editable in Subassembly composer.
This subassembly was created during a proCIVIL project which is not alive anymore.

This is a conditional subassembly which takes an input from previous subassembly and compares it with a condition parameter.

## Usage

Check out an [old proCivil video tutorial](https://youtu.be/B6fqmSYpDMs) in Czech language only :) funny history

### How to combine with Subassembly composer conditions ?

1.  Create a custom condition subassembly in Subassembly composer (SAC) with a output parameter - the output parametr must be DOUBLE type
2.  Reference the output parameter to "Input" of YesNoSwitch
3.  Set up desired output in YesNoSwitch to compare with referenced output from Subassembly composer. Set up the condition.
4.  next subassemblies will calculate itself only if YesNoSwitch Condition = Input parameter

## You can also watch

Want to know more about conditions and experimental subassemblies? There is a great speach on Autodesk university from Chino Que. [Check it out...](https://www.autodesk.com/autodesk-university/class/Civil-3D-Smart-Assembly-Using-Parametric-Design-to-Build-One-Assembly-for-All-2023)

## Parameters

Check out the [video](https://youtu.be/B6fqmSYpDMs)

| Name             | Type   | Description                                                                                   |
| ---------------- | ------ | --------------------------------------------------------------------------------------------- |
| Vstupní parametr | double | Input (referenced parameter)                                                                  |
| Podmínka         | double | Condition for Input - next subassembly is calculated only if "Condition" == "Input parameter" |
| Šířka rozvržení  | double | Width - Appearence for composing the assembly                                                 |
| Výška rozvržení  | double | Height - Appearence for composing the assembly                                                |

## Codes

-

### Points

-

### Lines

-

### Shapes

-

## Versions

| Version    | Date       | Description                           |
| ---------- | ---------- | ------------------------------------- |
| 2020 1.0.0 | 2024-09-23 | First release in pktFragments project |
|            |            |                                       |
