# PKGAssistant

PKGAssistant is a Python desktop application that simplifies the process of downloading and extracting PlayStation package files. With a user-friendly GUI and a command-line interface, users can easily specify line ranges from a TSV file, choose to automatically apply zRIF keys, and store the extracted files in a single ZIP archive.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
  - [GUI](#gui)
  - [Command-line](#command-line)
- [TSV Files](#tsv-files)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Installation

To use PKGAssistant, first clone the repository to your local machine:

```bash
git clone https://github.com/username/pkgassistant.git
cd pkgassistant
```

Then, install the necessary dependencies:

```bash
pip install -r requirements.txt
```

**Note**: PKGAssistant requires [pkg2zip](https://github.com/mmozeiko/pkg2zip) to be downloaded on your system to automatically apply zRIF keys.

## Usage

PKGAssistant can be used either through its GUI or command-line interface.

### GUI

To start the GUI, run:

```bash
python gui.py
```

This will open a window that allows you to select a TSV file, specify line ranges, and choose various options for downloading and extracting packages.

### Command-line

To use PKGAssistant from the command-line, run:

```bash
python main.py [ranges] [tsv_file] [-x] [-z] [-q] [--nogui]
```

- `[ranges]`: Line ranges in the format `4,5,8` or `4-8`.
- `[tsv_file]`: TSV file to read.
- `-x`: Delete files after unpacking.
- `-z`: Automatically apply zRIF key.
- `-q`: Store all files in a single ZIP file.
- `--nogui`: Start the command-line interface instead of the GUI.

## TSV Files

The TSV files used by PKGAssistant are not included in this repository and are not created by me. They are obtained from various sources on the internet and are used for educational purposes only. I do not claim ownership of any of the TSV files used by PKGAssistant.

## Acknowledgements

PKGAssistant uses the [pkg2zip](https://github.com/mmozeiko/pkg2zip) tool created by Maximiliano O. Martinez to automatically apply zRIF keys. I would like to thank Maximiliano for creating such a useful tool and making it available to the public.

## License

PKGAssistant is licensed under the GNU License. Please see the [LICENSE](LICENSE) file for more details.
