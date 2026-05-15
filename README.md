# miniscript

miniscript is a lightweight, indentation-based scripting language inspired by gdscript, built using c# and .net 8.

## features

- indentation-based block syntax (like python/gdscript)
- dynamic typing (numbers, strings, booleans, null)
- first-class functions and closures
- while loops and if/else statements
- built-in functions with standard library support.

## architecture

the project is divided into modular components:

- **lexer**: converts raw text into tokens while tracking indentation levels.
- **parser**: a recursive descent parser that builds an abstract syntax tree (ast).
- **ast**: immutable nodes with c# records.
- **runtime**: a tree-walking interpreter that manages scope and execution.

## getting started

1. `npm install -g @vscode/vsce`
2. `vsce package`
3. `code --install-extension msl-0.0.1.vsix`

## example syntax

```python
func greet(name):
    print("hello " + name)

var count = 0
while count < 3:
    greet("developer")
    count = count + 1
```

you can see more examples in the `MiniScript.Interp/samples` folder.

## license

this project is mit licensed, open-source and intended for educational purposes.
