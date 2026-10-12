# Aevix Language

**Syntax highlighting, snippets, and file icons for the Aevix programming language.**

Lightweight, zero-config support for `.aev` files — open a file and start coding.

## Install

1. Press `Cmd+Shift+X` (macOS) or `Ctrl+Shift+X` (Windows/Linux) to open the Extensions view
2. Search for **Aevix**
3. Click **Install**

Or from the terminal:

```bash
code --install-extension aevix.aevix-language
```

That's it — updates are installed automatically.

## Features

- **Syntax Highlighting** — Aevix keywords, types, functions, operators, and comments are colored out of the box
- **Snippets** — code templates for common constructs (`func`, `let`, `if`, `while`, `for`, `hot`, `print`)
- **File Icons** — a dedicated icon for `.aev` files in the explorer
- **Language Configuration** — auto-closing brackets, comment toggling (`//`), and bracket matching

## Example

```aev
import "lib/geometry";

struct Point { x: int, y: int }

func add(a: int, b: int) : int {
    return a + b;
}

if (x > 5) {
    print x;
} else {
    print 0;
}

for item in arr {
    print item;
}

// Hot regions and arenas
hot {
    let buf = new int[16];
    epoch {
        let tmp = new int[100];
    }
    print len(buf);
}
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

## Requirements

- VS Code 1.85.0 or higher

## Links

- [Aevix Language documentation](https://github.com/AevixLang/Aevix/blob/main/Syntax.md)
- [Source code](https://github.com/AevixLang/Aevix-VSCode)
- [Report an issue](https://github.com/AevixLang/Aevix-VSCode/issues)

## License

Apache License 2.0
