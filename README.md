# CPP

[https://www.mingw-w64.org](https://www.mingw-w64.org)

[https://github.com/niXman/mingw-builds-binaries/releases](https://github.com/niXman/mingw-builds-binaries/releases)

# MinGW

MinGW，是Minimalist GNU for Windows的缩写。它是一个可自由使用和自由发布的Windows特定头文件和使用GNU工具集导入库的集合，允许你在GNU/Linux和Windows平台生成本地的Windows程序而不需要第三方C运行时（C Runtime）库。MinGW 是一组包含文件和端口库，其功能是允许控制台模式的程序使用微软的标准C运行时（C Runtime）库（MSVCRT.DLL）,该库在所有的 NT OS 上有效，在所有的 Windows 95发行版以上的 Windows OS 有效，使用基本运行时，你可以使用 GCC 写控制台模式的符合美国标准化组织（ANSI）程序，可以使用微软提供的 C 运行时（C Runtime）扩展，与基本运行时相结合，就可以有充分的权利既使用 CRT（C Runtime）又使用 WindowsAPI功能。

# 编译器 MinGW 版本

‌MSVCRT（Microsoft Visual C++ Runtime）和UCRT（Universal C Runtime）是Microsoft Windows操作系统中两种不同的C标准库变体，它们在功能、兼容性和使用场景上有所不同。‌

功能和兼容性
‌MSVCRT‌：MSVCRT是微软提供的较老的C运行时库，它在所有Microsoft Windows版本中都默认可用。然而，由于向后兼容性问题，MSVCRT不支持C99标准，并且缺少一些功能，例如printf()函数族。此外，MSVCRT不支持UTF-8语言环境，这意味着与MSVCRT链接的二进制文件不应与使用UCRT链接的二进制文件混合使用，因为它们的内部结构和数据类型不同‌12。
‌UCRT‌：UCRT是较新的C运行时库，也是Microsoft Visual Studio默认使用的版本。UCRT与MSVC（Microsoft Visual C++）编译的代码兼容性更好，无论是在构建时还是在运行时。UCRT默认在Windows 10上提供，对于较早的Windows版本，用户需要自己提供或依赖安装了UCRT的用户‌12。
使用场景
‌MSVCRT‌：由于MSVCRT在所有Windows版本上都可用，它适用于需要广泛兼容性的场景。然而，由于它的限制和兼容性问题，对于需要使用最新C标准或特定语言环境的项目，MSVCRT可能不是最佳选择。
‌UCRT‌：UCRT是较新的标准库，支持最新的C标准（如C11），并且与MSVC编译的代码有更好的兼容性。因此，它适用于需要利用最新C标准功能和与MSVC编译代码兼容的项目，特别是在Windows 10及更高版本的操作系统上‌12。
综上所述，‌MSVCRT和UCRT在功能、兼容性和使用场景上有显著区别‌。选择合适的运行时库取决于项目的具体需求和目标平台。