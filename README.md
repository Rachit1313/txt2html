<h1 align="center">txt2html</h1>

<div align="center">
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

</div>

## Features

- This is a command-line tool process input txt files output html files.
- Allow the user to specify either a file or folder of files as input

### Markdown Conversions
- This command-line tool enables the following Markdown conversions to HTML:
  - Paragraphs (blank-line separated) are transformed to \<p>Paragraph Content\</p>
  - Italics (\*word\* or \_word\_ to \<i>word\</i>)

### Planned features
- [x] User specified output path (version 0.1.1)
- [x] Set title from input file content (version 0.1.2)
- [x] Support Markdown file input and Italics Parsing (version 0.1.3)
- [x] Add support for Markdown horizontal rule (`---`) to convert that to an `<hr>` tag. Support language attribute configuration (version 0.1.4)
## How to Install 

**In command line:**

Make sure python3 is installed:
```bash
python3 --version
```

Clone the Repo

```bash
git clone https://github.com/mingming-ma/txt2html.git
cd txt2html 
```

Make the tool executable
```bash
chmod +x txt2html.py
```
## Usage

To generate html from a txt file: 
```bash
./txt2html.py input_file.txt
```
To generate html from a folder which has txt files: 
```bash
./txt2html.py folder-name
```

## Command Flags

<!-- Available command options:
```
-v,--version - Displays the version of the tool
-h,--help - Displays the help message
``` -->

| Command   | Description |
| --------- | ----------- |
| -h, --help | Displays the help message |
| -v, --version | Displays the version of the tool |
| -o, --output | Specify the output directory. Existing output folder will first be removed. If not specified, "./txt2html" will be used.|
| -l, --lang | Specify the language to use when generating the lang attribute on the root <html> element. If not specified, "en-CA" will be used.|