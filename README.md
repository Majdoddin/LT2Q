# LTSpice to QSpice Circuit Converter

**lt2q.majdoddin.com** - The first automated online service for converting LTSpice circuit files (.asc) to QSpice format (.qsch) with instant results.

## What it does

- **Converts circuit files**: Takes LTSpice .asc files and outputs QSpice .qsch files
- **Preserves circuit integrity**: Maintains all components, wires, junctions, net labels, and TEXT elements
- **Handles complex graphics**: Converts symbol libraries, rotations, and coordinate systems
- **Supports advanced features**: Processes SPICE directives, comments, model definitions, and Unicode characters

## Key features

- **Complete conversion**: Components, wires, junctions, net labels, and annotations
- **Symbol library integration**: Embeds LTSpice symbol graphics directly into QSpice format
- **Encoding support**: Handles special characters like µ symbols
- **Model definitions**: Automatically processes multi-line SPICE models
- **Wire connectivity**: Graph-based algorithm preserves electrical connections

The converter solves the problem of migrating circuits between these two popular SPICE simulation platforms, saving engineers significant time and effort.

## TODO

- **Subcircuit conversion**: Support for LTSpice subcircuit (.sub) files
- **Replace LTspice STARTUP with QSPICE UEC**: See the discussions [here](https://forum.qorvo.com/t/yet-another-ltspice-conversion-support-request-ti-tps7a85/22697) and [here](https://forum.qorvo.com/t/startup-seems-to-be-ignored-by-qspice-in-the-trans-command/1662)
- **Handle Rser/Lser parameters**: These are intentionally not implemented in QSPICE - see [here](https://forum.qorvo.com/t/why-doesnt-qspice-support-series-inductance-in-the-cpacitor-model/17470) and [here](https://forum.allaboutcircuits.com/threads/ltspice-spiceline-parameters.201802/)
- **IGBT symbol conversion**: IGBT symbols exist in LTSpice but not in QSPICE
- **Laplace expression limitations**: QSPICE cannot handle transcendental functions like exp() in Laplace expressions - see [here](https://forum.qorvo.com/t/laplace-expression-syntax/14962)
- **STEP PARAM with model parameters**: QSPICE requires different approach for parameter stepping in SPICE models compared to LTSpice - see [here](https://forum.qorvo.com/t/step-param-with-parametre-into-spice-model/17836)

## Contributing

Found a bug or have a feature request? Please add an issue to help us improve the converter.