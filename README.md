# C++ learning repo

Small chapter-by-chapter exercises and notes while learning C++. Each folder is one topic; source files are meant to be compiled and run locally.

## Quick start

From any `.cpp` file:

```bash
g++ -std=c++17 -Wall -o program program.cpp
./program
```

On macOS, `g++` is typically Apple Clang. Use `-std=c++17` (or newer) for `string` and modern features without extra flags.

## Chapters

### Chapter 1 — Intro (`chapter1-intro/`)

Getting comfortable with a minimal program, `iostream`, and reading input.

| File | What it covers |
|------|----------------|
| `hello2.cpp` | `main`, `cout` / `cin`, `string`, greeting the user by first name |
| `cin.cpp` | Variable declarations: `int`, `float`, `char`, `bool`, `const double` (snippet, not a full program) |
| `testfile-only/nameinput.cpp` | Same input pattern as `hello2.cpp` with a slightly different greeting |

Local build artifacts (e.g. `hello2`, `cin`, `variables`) may exist after compiling; prefer compiling from the `.cpp` sources.

### Chapter 2 — Variables & data types (`chapter2-variables-datatypes/`)

Output with `cout` and mixing text with numeric values.

| File | What it covers |
|------|----------------|
| `basic-io.cpp` | `cout`, `endl`, printing strings and integers |
| `input.cpp` | Work in progress — intended to extend basic I/O |

### Chapter 3 — Escape sequences (`chapter3-scape-sequence/`)

Special characters in strings (`\n`, `\t`, `\"`, etc.) and formatted output.

| File | What it covers |
|------|----------------|
| `escape.cpp` | Started as input practice (`scanf`); folder name targets escape sequences — good place to add `\n`, `\t`, and quoted strings |

### Type casting (root)

| Path | What it covers |
|------|----------------|
| `type-casting/` | Placeholder for implicit/explicit casts, `static_cast`, and numeric conversions |

## Suggested order

1. `chapter2-variables-datatypes/basic-io.cpp` — simplest output-only program  
2. `chapter1-intro/hello2.cpp` — add user input  
3. `chapter1-intro/cin.cpp` — read types and constants (paste into a small `main` if you want to run it)  
4. `chapter3-scape-sequence/` — escape sequences and neat formatting  
5. `type-casting/` — when you mix types and need safe conversions  

## Repo layout

```
cpp/
├── README.md
├── chapter1-intro/
├── chapter2-variables-datatypes/
├── chapter3-scape-sequence/
└── type-casting/
```

Personal study notes (how to learn C++, resources, schedule) live in a local-only file listed in `.gitignore` — see `HOW-TO-LEARN-CPP.md` in your working copy after you create or restore it from your machine.
