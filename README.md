# Aevix Language for VS Code

**Syntax highlighting, snippets, and file icons for the Aevix programming language.**

## Features

- **Syntax Highlighting** — Full support for Aevix keywords, types, functions, operators, and comments
- **Snippets** — Quick code templates for common constructs (`func`, `let`, `if`, `while`, `for`, `hot`, `print`)
- **File Icons** — Custom `.aev` file icon in the explorer
- **Language Configuration** — Auto-closing brackets, comment toggling, bracket matching

## Supported Syntax

```aev
// Variables
let x: int = 10;
let y = 20.5;

// Functions
func add(a: int, b: int) : int {
    return a + b;
}

// Control Flow
if (x > 5) {
    print x;
} else {
    print 0;
}

for (let i = 0; i < 10; i = i + 1) {
    print i;
}

while (x > 0) {
    x = x - 1;
}

// Hot Regions (performance-critical)
hot {
    let t = x + 1;
    print t;
}

// Arrays
let arr = [1, 2, 3];
print arr[0];
```

## Snippets

| Prefix | Description |
|--------|-------------|
| `func` | Define a new function |
| `let` | Declare a variable |
| `if` | If-Else conditional |
| `while` | While loop |
| `for` | Standard for loop |
| `forin` | For-In loop |
| `hot` | Performance-critical hot region |
| `print` | Print a value to console |

## Installation

### From VSIX

1. Download the latest `.vsix` file from [Releases](https://github.com/OsmanNuri/Aevix-VSCode/releases)
2. Open VS Code
3. Press `Cmd+Shift+P` (macOS) or `Ctrl+Shift+P` (Windows/Linux)
4. Type "Install from VSIX" and select the downloaded file

### From Source

```bash
git clone https://github.com/OsmanNuri/Aevix-VSCode.git
cd Aevix-VSCode
npm install
vsce package
# Install the generated .vsix file
```

## Requirements

- VS Code 1.85.0 or higher

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Links

- [Aevix Language Repository](https://github.com/OsmanNuri/Aevix-Language)
- [Aevix Documentation](https://github.com/OsmanNuri/Aevix-Language/blob/main/Syntax.md)
- [Report Issues](https://github.com/OsmanNuri/Aevix-VSCode/issues)
