# GrainPrint
A beautified print function for grain, similar to the original grain print it works on any type.

## Features
* Colored Printing
* Line Breaks
* Custom Byte Limit
* Custom Depth Limits
* Custom Ident Amount

## Note
Grain v0.6 has added cycle support to the native `print` function, this library does not currently support cycle detection.

## TODO
* Make A PrintTree, This allows for faster support of line breaks and more complex line breaking mechanics surrounding nesting
* Detect support for colors
* Create Fall back to basic ascii colors over true color
* Add a compact mode
* Cycles Support
* Simply Package by separating type logic from printing (This would give an opportunity to improve type safety)
  * We could have this be a separate package because it could be pretty useful
  * I'm picturing a serialization package, that converts the adts, enums and records over to a data representation
* Check For Memory Leaks
* Remove dependencies on stdlib and Pervasives
* Write Grain Doc
* Support Custom Printing Radix