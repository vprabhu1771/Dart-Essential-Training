# 1 - Installing the Dart SDK

```
https://dart.dev/get-dart
```

You can install the Dart SDK using Chocolatey.

Important: These commands require administrator rights. Here’s one way to open a Command Prompt window that has admin rights:

1) Press Windows+R to open the Run window.
   
2) Type cmd into the box.
   
3) Press Ctrl+Shift+Enter.


To install the Dart SDK:

```
choco install dart-sdk
```

To upgrade the Dart SDK:

```
choco upgrade dart-sdk
```

By default, the SDK is installed at C:\tools\dart-sdk. You can change that location by setting the ChocolateyToolsLocation environment variable to your chosen installation directory.

If you can’t use the Dart SDK executables, add the SDK location to your PATH:

By default, the SDK is installed at C:\tools\dart-sdk. You can change that location by setting the ChocolateyToolsLocation environment variable to your chosen installation directory.

If you can’t use the Dart SDK executables, add the SDK location to your PATH:

    In the Windows search box, type env.
    Click Edit the system environment variables.
    Click Environment Variables….
    In the user variable section, select Path and click Edit….
    Click New, and enter the path to the dart-sdk directory.
    In each window that you just opened, click Apply or OK to dismiss it and apply the path change.


System requirements

The Dart SDK is supported on Windows, Linux, and macOS.
Windows

    Supported versions: Windows 10 and 11.
    Supported architectures: x64, IA32, ARM64.
    Support for ARM64 is experimental, and is available only in the dev channel.
