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

## Contributing

Found a bug or have a feature request? Please add an issue to help us improve the converter.