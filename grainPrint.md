---
title: GrainPrint
---

## Types

Type declarations included in the GrainPrint module.

### GrainPrint.**Radix**

```grain
enum Radix {
  Hex,
  Dec,
  Oct,
  Bin,
}
```

The Desired Printing Radix.

### GrainPrint.**PrintSettings**

```grain
record PrintSettings {
  colored: Bool,
  indentAmount: Number,
  maxDepth: Number,
  newLineChar: String,
  printSuffix: Bool,
  byteLimit: Number,
  rainbowBracket: Bool,
  radix: Radix,
  forceNewLine: Bool,
  newLineList: Option<Number>,
  newLineArray: Option<Number>,
  newLineRecord: Option<Number>,
  newLineTuple: Option<Number>,
}
```

Printing Settings.

`colored` - Wether to use colors or not.
`indentAmount` - How much to indent by each level.
`maxDepth` - The maximum depth to print.
`newLineChar` - The character to use for new lines.
`printSuffix` - Wether to print the suffix or not.
`byteLimit` - The maximum number of bytes to print.
`rainbowBracket` - Wether to use rainbow brackets or not.
`radix` - The radix to use for numbers.
`forceNewLine` - Wether to force new lines or not.
`newLineList` - The maximum length before we split list.
`newLineArray` - The maximum length before we split arrays.
`newLineRecord` - The maximum length before we split records.
`newLineTuple` - The maximum length before we split tuples.

## Values

Functions and constants included in the GrainPrint module.

### GrainPrint.**print**

```grain
print : (a: a, ?printSettings: PrintSettings) => Void
```

Prints the given operand to the console. Works for any datatype.

Parameters:

|param|type|description|
|-----|----|-----------|
|`a`|`a`|The operand to print.|
|`printSettings`|`Option<PrintSettings>`|The settings to use when printing.|

