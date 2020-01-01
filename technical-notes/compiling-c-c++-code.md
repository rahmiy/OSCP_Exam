# Compiling C/C++ code

## compiling c code for windows environment

Installing the cross-compilation

```text
sudo apt-get install mingw-w64
```

32bit

```text
i686-w64-mingw32-gcc -o test.exe test.c
```

64bit

```text
x86_64-w64-mingw32-gcc -o test.exe test.c
```

ref : [https://stackoverflow.com/questions/44670209/how-to-compile-c-code-in-linux-to-run-on-windows](https://stackoverflow.com/questions/44670209/how-to-compile-c-code-in-linux-to-run-on-windows)

