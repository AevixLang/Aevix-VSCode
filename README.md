# Aevix Language for VS Code

**Syntax highlighting, snippets, and file icons for the Aevix programming language.**

## Features

- **Syntax Highlighting** — Full support for Aevix keywords, types, functions, operators, and comments
- **Snippets** — Quick code templates for common constructs (`func`, `let`, `if`, `while`, `for`, `hot`, `print`)
- **File Icons** — Custom `.aev` file icon in the explorer
- **Language Configuration** — Auto-closing brackets, comment toggling, bracket matching

## Supported Syntax

```aev
// Imports
import "lib/geometry";

// Structs
struct Point { x: int, y: int }

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

for (let i = 0; i < 10; i += 1) {
    if (i == 3) { continue; }
    if (i == 6) { break; }
    print i;
}

for item in arr {
    print item;
}

while (x > 0) {
    x -= 1;
}

// Hot regions and epochs
hot {
    let buf = new int[16];
    epoch {
        let tmp = new int[100];
    }
    print len(buf);
}

// Arrays and slices
let arr = [1, 2, 3];
let a: int[4] = [1, 2, 3, 4];
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
| `epoch` | Arena rollback scope |
| `struct` | Define a struct |
| `import` | Import declarations from a file or package |
| `new` | Allocate a zeroed array in the arena |
| `break` / `continue` | Loop control |
| `print` | Print values to console |

## Installation

### From VSIX

1. Download the latest `.vsix` file from [Releases](https://github.com/AevixLang/Aevix-VSCode/releases)
2. Open VS Code
3. Press `Cmd+Shift+P` (macOS) or `Ctrl+Shift+P` (Windows/Linux)
4. Type "Install from VSIX" and select the downloaded file

### From Source

```bash
git clone https://github.com/AevixLang/Aevix-VSCode.git
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

- [Aevix Language Repository](https://github.com/AevixLang/Aevix)
- [Aevix Documentation](https://github.com/AevixLang/Aevix/blob/main/Syntax.md)
- [Report Issues](https://github.com/AevixLang/Aevix-VSCode/issues)
