# LoongArch Assembly

An extension that provides language support for LoongArch assembly language.

## Features

* Provide syntax highlighting for LoongArch assembly language.
* Provide support for comment shortcuts.

## Developing

```bash
# Install js-yaml as a development only dependency in your extension
$ npm install js-yaml --save-dev

# Use the command-line tool to convert the yaml grammar to json
$ npx js-yaml syntaxes/loongarch.tmLanguage.yaml > syntaxes/loongarch.tmLanguage.json

# Update package-lock.json
$ npm install

# Install vsce for packaging, publishing and managing VS Code extensions
$ npm install -g vsce

# Package the extension
$ vsce package
```

## Known Issues

* Comments starting with `#` must be followed by a whitespace character in order to be highlighted correctly.
* Highlighting of rarely used symbols may be missing or redundant.

## Release Notes

### 1.0.0

Initial release of loongarch-assembly.

Add syntax highlighting for LoongArch assembly language.

### 1.1.0

Add support for comment shortcuts.

### 1.1.1

Fix highlighting for terms like `$r0`.

### 1.1.2

Fix highlighting for comments like `// xxx: xxx`.

### 1.1.3

Change the minimum version of VS Code API that the extension depends on.

### 1.1.4

Fix highlighting for words like `kernelsp`.

Remove highlighting for registers not beginning with `$`.

### 1.2.0

Add highlighting for more escape sequences.

Add highlighting for FCSR registers.

Add highlighting for LVZ, LBT, LSX and LASX instructions.

### 1.2.1

Fix missing highlighting.

## Reference

* [Vscode Language Extensions, Syntax Highlight Guide](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide)
* [Language Grammars, Naming Conventions](https://macromates.com/manual/en/language_grammars#naming_conventions)
* [Regular Expressions](https://raw.githubusercontent.com/kkos/oniguruma/master/doc/RE)
* [LoongArch Opcodes](https://sourceware.org/git/?p=binutils-gdb.git;a=blob_plain;f=opcodes/loongarch-opc.c;hb=HEAD)
* [Assembler Directives](https://sourceware.org/binutils/docs/as/Pseudo-Ops.html)
* [Directives](https://gcc.gnu.org/onlinedocs/cpp/Index-of-Directives.html)
