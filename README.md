clang-format
============

[![Test](https://github.com/egor-tensin/clang-format/actions/workflows/test.yml/badge.svg)](https://github.com/egor-tensin/clang-format/actions/workflows/test.yml)

This GitHub action runs `clang-format` on your C/C++ source files and shows the
diff.

Use it in your workflow like this:

    - name: clang-format
      uses: egor-tensin/clang-format@v1

API
---

| Input   | Value   | Default | Description
| ------- | ------- | ------- | -----------
| version | *empty* | ✓       | Use `clang-format`.
|         | *any*   |         | Use `clang-format-VERSION`.
| style   | file    | ✓       | Use .clang-format.
|         | *any*   |         | `-style=STYLE` (Microsoft, LLVM, etc.).
| exclude | *empty* | ✓       | Don't exclude any files.
|         | *any*   |         | List of files and directories to exclude, separated by a colon `:`.

| Output | Description
| ------ | -----------
| diff   | Diff between the original and the properly formatted files.

License
-------

Distributed under the MIT License.
See [LICENSE.txt] for details.

[LICENSE.txt]: LICENSE.txt
