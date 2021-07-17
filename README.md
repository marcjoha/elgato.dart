# elgato.dart

CLI to interact with Elgato Lights on the local network.

## How?

This project is written in Dart, and can probably be compiled on any
platform that Dart supports (Windows, Linux, macOS).

```shell
# Clone this repo 
git clone https://github.com/marcjoha/elgato.dart.git

# Enter the directory
cd elgato.dart

# Compile to native code:
dart compile exe elgato.dart

# Exceute the resulting binary
./elgato.exe
```

Instructions are available in ``--help``:

```shell
Usage: elgato.dart <command> [arguments]

Global options:
-h, --help    Print this usage information.

Available commands:
  decrease   Decrease brightness or temperature of each light.
  increase   Increase brightness or temperature of each light.
  off        Switch light(s) off.
  on         Switch light(s) on.
  toggle     Toggle switch of each light. [Default]

Run "elgato.dart help <command>" for more information about a command.
```

## Credits

This is originally a fork of [Mike Fiedler's project](https://github.com/miketheman/elgato.dart),
but has changed considerably to fit my workflow (and code preferences). Please consider trying out
Mike's project first, to see if it fits your needs. If you need more powerful command switches, this
project might be what you're looking for.

In turn, Mike's project was inspired by [Brett Langdon](https://github.com/brettlangdon), who had
figured out how to control the lights via Bash, while using static IP
addresses. Mike took the idea further and wrote a Dart application that can discover
lights on the network automatically.
