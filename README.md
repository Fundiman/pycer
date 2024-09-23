# Pycer - A Simple Package Manager Script 

**Pycer** is a simple command-line package manager script for installing and uninstalling Python packages. It supports multiple sources such as `pip`, `conda`, `poetry`, `pipenv`, `pipx`, `flit`, and `hatch`, as well as direct URLs for downloading packages.

## Features

- Install packages from known sources (`pip`, `conda`, `poetry`, `pipenv`, `pipx`, `flit`, `hatch`).
- Install packages from direct URLs.
- Uninstall packages by removing their directories.

## Installation

To use Pycer, you need Python 3 installed on your system. You also need the following Python packages:

- `requests`

You can install the required packages using `pip`:

```bash
pip install requests
```

## Usage

### Installing a Package

You can install a package either from a known source or from a direct URL.

#### From a Known Source

To install a package from a known source, use the following command:

```bash
python3 pycer.py install {lib} from {source}
```

- `{lib}`: The name of the library you want to install.
- `{source}`: The known source (e.g., `pip`, `conda`, `poetry`, `pipenv`, `pipx`, `flit`, `hatch`).

Example:

```bash
python3 pycer.py install requests from pip
```

#### From a Direct URL

To install a package from a direct URL, use the following command:

```bash
python3 pycer.py install {lib} from {url}
```

- `{lib}`: The name of the library you want to install.
- `{url}`: The URL to the package file.

Example:

```bash
python3 pycer.py install requests from https://example.com/requests.zip
```

### Uninstalling a Package

To uninstall a package, use the following command:

```bash
python3 pycer.py uninstall {lib}
```

- `{lib}`: The name of the library you want to uninstall.

Example:

```bash
python3 pycer.py uninstall requests
```

## Requirements

- Python 3
- `requests` library

## Notes

- For known sources (`pip`, `conda`, etc.), the script uses predefined commands to perform the installation.
- Direct URLs should point to files in supported formats (`.zip`, `.tar.gz`, `.tgz`, `.whl`).
- If the file format is not recognized, the file will be saved in the current directory.
- This tool is in development so be careful while using it.

## Publishing Packages
To publish any package; 
1. Go to the discussion tab
2. Goto group publish
3. Send your url
4. After sometime, you should see your url be in pycer-repos.txt

## Contributing

Feel free to contribute to the project by submitting issues or pull requests. Your feedback and suggestions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

----------------------------
Project Status: Comming soon
