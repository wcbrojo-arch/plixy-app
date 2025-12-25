Plixy — minimal toy programming language (Node.js implementation)

Quickstart

- Install (optional): `npm install -g .`
- Run the REPL: `npx plixy-repl` or `node bin/repl.js`
- Run a file: `node bin/repl.js examples/hello.plx`

Windows quick launcher

- From this project folder you can run `tx` via the provided `tx.cmd`:

```powershell
.\tx.cmd examples/hello.plx
```

- After `npm install -g .` the `tx` command will be available globally.

Language highlights
- `let <name> = <expr>` — assign variable
- `print <expr>` — print expression
- `say <word>` or `say "text"` — print a word or string to console (convenience for quick messages)

- Bare expressions: writing an expression as a statement prints its value. Example: `1+1` will print `2`.

- Functions: define with `fn` and `end`. Parameters go inside parentheses (space-separated). Use `return` to return a value.

Example:

```
fn add(a b)
	return a + b;
end

say add(1 2);
```
- `if <expr> then ... else ... end` — conditional
- `while <expr> do ... end` — loop

This is a minimal interpreter for experimentation. If you want a different runtime (Rust, Go, etc.), tell me and I can scaffold that instead.
