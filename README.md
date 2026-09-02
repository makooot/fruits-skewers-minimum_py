# fruits-kewers-minimum

> ⚠️ **Disclaimer: This is a learning-oriented project.**
> This repository is built strictly for personal learning and practicing Python library development. It is **not actively maintained for public production use**. Bug reports, feature requests, or Pull Requests may not be reviewed or addressed. Feel free to fork the repository for your own use under the MIT License.

Command line argument parser

## Installation

coming soon

## Quick Start

Here is a simple example of how to use the library:

```python
from fruits_skewers_minimum import parser_minimum as skewer

try:
    result = skewer.parser()
except skewer.types.ShowHelpException:
    print("usage: COMMAND OPTIONS")
    exit(0)
except skewer.types.ShowVersionException:
    print("COMMAND 0.0.0")
    exit(0)

if "verbose" in result:
    if "host" in result:
        print(f"Host: {result.get('host')}")
    else:
        print("Host: (default) ")
    if "port" in result:
        print(f"Port: {result.get('port')}")
    else:
        print("Port: (default) ")
argv = result.get("ARGV")
print(f"ARGV: {len(argv)}")
for i, arg in enumerate(argv):
    print(f"  [{i}]: {arg}")
```

## Contributing

Please refer to CONTRIBUTING.md for details on how this repository handles issues, pull requests, and forks.

## License

MIT License
