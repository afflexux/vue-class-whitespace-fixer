![npm](https://img.shields.io/npm/v/vue-class-whitespace-fixer)
![license](https://img.shields.io/npm/l/vue-class-whitespace-fixer)
![downloads](https://img.shields.io/npm/dt/vue-class-whitespace-fixer)
![downloads](https://img.shields.io/npm/dw/vue-class-whitespace-fixer)
![downloads](https://img.shields.io/npm/dm/vue-class-whitespace-fixer)
![GitHub last commit](https://img.shields.io/github/last-commit/afflexux/vue-class-whitespace-fixer)

# vue-class-whitespace-fixer

A tool to fix excessive whitespace in class attributes of Vue files.

## Description

`vue-class-whitespace-fixer` is a simple tool that helps clean up excessive whitespace in class attributes of Vue files. This is especially useful for projects using TailwindCSS, where class names can get quite long and whitespace management is important for readability and maintenance.

While the TailwindCSS Prettier plugin now removes excessive whitespace, the ESLint TailwindCSS plugin does not yet offer this functionality. `vue-class-whitespace-fixer` fills this gap by ensuring your Vue files have clean, consistent class attributes without excessive whitespace.

## Installation

To install `vue-class-whitespace-fixer`, run:

```bash
npm install -g vue-class-whitespace-fixer
````
This will install the tool globally, allowing you to use it from anywhere on your system.

## Usage

After installing the tool, you can run it from the command line. You need to provide the path to the directory containing your Vue files. If no directory is provided, the tool will default to the current directory.

### Running the Tool

To run the tool on a specific directory:

```bash
vue-class-whitespace-fixer /path/to/your/vue/project
````

To run the tool in the current directory:

```bash
vue-class-whitespace-fixer .
````

### Example

```bash
vue-class-whitespace-fixer /Users/yourname/projects/my-vue-app
````

This command will traverse through the specified directory, process all Vue files, and fix excessive whitespace in their class attributes.

### Output

The tool will output the following information to the terminal:

*   The paths of the files that have been changed.
*   The total number of Vue files processed.
*   The number of files that have been changed.

### Notes

*   The tool will skip processing for `:class` bindings as they often include dynamic expressions where whitespace could be intentional or necessary.
*   The `node_modules` directory is automatically excluded from processing.

## License

This project is licensed under the ISC License.

## Author

Afflexux
