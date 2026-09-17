# AMD BC-250 Custom Cooling Build

[한국어](README.md)

This document records a custom cooling configuration for the AMD BC-250 using a standard AMD CPU cooler, 3D-printed mounts, and a rear 120 mm fan instead of the original large heatsink assembly.

It focuses only on **parts and assembly structure**, not benchmark results or current operating status.

## Parts Used

| Item | Part / File |
|---|---|
| Board | AMD BC-250 |
| CPU cooler | **DeepCool AG400 G2** |
| CPU cooler mount | `bc250-am5-mount-7mm-bi.step` |
| Rear 120 mm fan adapter | `maurice56-jfk13k-clamping-plate-120mm-fan.stl` |
| Rear fan spacer | `maurice56-jfk13k-fan-spacer.stl` or a suitable substitute |
| Rear cooling | Standard 120 mm fan |
| Backplate heatsink | **Reuse the original BC-250 backplate heatsink as-is** |

## 3D Models Used

### AM5 7 mm Mount

File used:

```text
bc250-am5-mount-7mm-bi.step
```

Original model:

- **AM5 CPU cooler mount for the BC250**
- Author: **Gadget**
- Printables: https://www.printables.com/model/1826539-am5-cpu-cooler-mount-for-the-bc250
- Version used: **7 mm**

This mount allows a standard AMD CPU cooler mounting bracket to be installed on the BC-250.

For the DeepCool AG400 G2, use the AMD metal mounting bracket supplied with the cooler. The orange AMD spacers supplied with the cooler are not used in this build.

### Rear 120 mm Fan Adapter

Files used:

```text
maurice56-jfk13k-clamping-plate-120mm-fan.stl
maurice56-jfk13k-fan-spacer.stl
```

Original project:

- **BC-250 Mount for Jiushark JF13K (VRM Airflow Directed)**
- Author: **Maurice56**

This build does not use the complete JF13K mounting system. Only the **rear clamping plate / 120 mm fan adapter** is used.

The printed fan spacers may be replaced with suitable alternatives. In this build, spacers included with the CPU cooler were used instead.

## Recommended Screws and Fasteners

Whenever possible, using **M3 screws with nuts** is recommended.

| Purpose | Recommended size | Quantity |
|---|---:|---:|
| Rear 120 mm fan mounting | M3 × 50 mm | 4 |
| Rear fan adapter ↔ AM5 7 mm mount | M3 × 25 mm | 4 |
| AM5 7 mm mount ↔ CPU cooler AMD bracket | M3 × 20 mm | 4 |

Matching **nuts and washers** are also required.

> The current build uses **M4 × 25 mm** screws between the rear fan adapter and the AM5 7 mm mount. The printed mount holes were enlarged to approximately 4 mm with a drill. If building from scratch, M3 hardware is easier because no additional hole enlargement is required.

## Assembly Structure

### 1. Rear 120 mm Fan Connection

Fastener order:

```text
120 mm fan
↓
nut
↓
spacer
↓
nut
↓
120 mm fan adapter mount
↓
M3 × 50 mm screw head
```

- Use **4 × M3 × 50 mm** screws
- The dedicated printed spacers may be replaced with suitable alternatives
- In this build, spacers included with the CPU cooler were used

### 2. Rear Fan Adapter ↔ AM5 7 mm Mount

This connection joins the rear fan adapter to the AM5 7 mm mount on the front side of the PCB.

**The original BC-250 backplate heatsink is left in place and reused as-is. It is not removed or modified.**

In this build, each screw is first inserted through the rear fan adapter and then **locked to the fan adapter with a nut**. The assembly is then passed through the original backplate heatsink and the PCB.

Current fastener order:

```text
M4 × 25 mm screw head
↓
120 mm fan adapter mount
↓
nut  ← locks the screw to the fan adapter first
↓
original BC-250 backplate heatsink (reused as-is)
↓
original BC-250 spring
↓
original BC-250 plastic washer
↓
BC-250 PCB
↓
AM5 7 mm mount
↓
washer
↓
nut
```

The current build uses **4 × M4 × 25 mm** screws, which required enlarging the printed mount holes with a drill.

For a new build, **4 × M3 × 25 mm** screws are recommended because they are easier to work with.

Reuse the **original BC-250 springs and plastic washers**.

### 3. AM5 7 mm Mount ↔ CPU Cooler AMD Bracket

Fix the AMD metal mounting bracket supplied with the CPU cooler onto the AM5 7 mm mount.

Fastener order:

```text
M3 × 20 mm screw head
↓
AM5 7 mm mount
↓
CPU cooler AMD mounting bracket
↓
washer
↓
nut
```

Use **4 × M3 × 20 mm** screws.

The screw heads must not protrude above the surface of the AM5 7 mm mount. If they stick out, they may interfere with the CPU cooler, so the heads should be recessed into the mount.

### 4. CPU Cooler Installation

After the AMD metal bracket is fixed to the AM5 7 mm mount, install the CPU cooler itself using the cooler's normal AMD mounting method.

This build uses a **DeepCool AG400 G2**.

```text
BC-250 PCB
↓
AM5 7 mm mount
↓
AG400 G2 AMD metal mounting bracket
↓
AG400 G2 cooler
```

Because the BC-250 exposes the CPU/APU die directly, tighten the cooler gradually and evenly. Avoid fully tightening one side before the other.

## Fastener Summary

```text
M3 × 50 mm × 4
M3 × 25 mm × 4   # recommended; current build uses M4 × 25 mm × 4
M3 × 20 mm × 4

nuts / washers
original BC-250 springs × 4
original BC-250 plastic washers × 4
spacers × 4
```

## Recommended 3D Printing Materials

Because the mounts may be exposed to heat from the board and nearby power components, the following materials are recommended over PLA:

- PETG
- ABS
- ASA
- PC

## Credits

This build is based on 3D models created by the following authors:

- Gadget — **AM5 CPU cooler mount for the BC250**
- Maurice56 — **BC-250 Mount for Jiushark JF13K (VRM Airflow Directed)**

Check the license of each original project before redistributing or modifying the models.
