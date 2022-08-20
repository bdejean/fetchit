<div align="center">

<img src="https://user-images.githubusercontent.com/56625259/185757248-cb60e3e8-9486-41dc-9e99-f0f24a208e71.png" width="457" height="259">

# fetchit

A system fetch tool for Linux, written in ***Rust***.

</div>

`fetchit` is a simple system info tool, written in *Rust*, for Linux based operating systems. It offers a few customization options, which are demonstrated in the
screenshots below,
- You can change the colors for the ***top*** and ***bottom*** part of the ascii art, as well as the color for the ***bounding box***.
- The path to a custom ascii text file can be passed to `fetchit` using the `-f` option.

For a custom ascii text file, it is recommended that the ascii art should be contained in a box of `10x28`, i.e. `28` ***spaces*** wide, and `10` ***lines***
in height. If this condition is not met (especially, the height, i.e. the number of lines) then `fetchit` will fall back to the default ascii asrt. See [Usage](https://github.com/Ruturajn/fetchit/edit/main/README.md#usage) for more details.

## Examples

<div align="center">

<img src="https://user-images.githubusercontent.com/56625259/185761191-26002c20-b4a4-43cd-929d-a55dcacff9c3.png" width="445" height="201"> &nbsp; <img src="https://user-images.githubusercontent.com/56625259/185761191-26002c20-b4a4-43cd-929d-a55dcacff9c3.png" width="445" height="201">

<img src="https://user-images.githubusercontent.com/56625259/185761450-3251ad79-ce36-4441-bb96-52781ab06828.png" width="464" height="204">

<br>

</div>

<br>

## Installation

You can install `fetchit` using any of the following methods,

### Install from Releases

### Building from Source
```
# Clone the git repo.
$ git clone https://github.com/Ruturajn/fetchit.git

# Change directory into the repo.
$ cd ./fetchit

# Build the package.
$ cargo build --release

# Create ~/.cargo/bin/ if it does not exist
$ if [[ ! -d ~/.cargo/bin ]] ; then mkdir -p ~/.cargo/bin/ ; fi

# Copy the executable to 
$ cp ./target/release/fetchit ~/.cargo/bin/
```

## Usage
```
fetchit 0.1.0
Ruturajn <nanotiruturaj@gmail.com>
A System fetch tool for Linux written in Rust

USAGE:
    fetchit [OPTIONS]

OPTIONS:
    -b, --bottom-color <BOTTOM_COLOR>
            Color for the bottom part of the ascii art : black, red, yellow, blue, magenta, cyan,
            white, green

    -f, --file-path <FILE_PATH>
            File path for the ascii text file

    -h, --help
            Print help information

    -o, --outer-box-color <OUTER_BOX_COLOR>
            Color for the box : black, red, yellow, blue, magenta, cyan, white, green

    -t, --top-color <TOP_COLOR>
            Color for the top part of the ascii art : black, red, yellow, blue, magenta, cyan,
            white, green

    -V, --version
            Print version information
```

## References
- https://github.com/anhsirk0/fetch-master-6000
