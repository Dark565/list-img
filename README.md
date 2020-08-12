# term-img - Print images from stdin to a terminal

## Content
This repository contains two scripts in src/:

- term-img
- list-img

The first one is used to print an image in a terminal with specified position and size.  It is used by list-img.  
The second one is the title script, used to print images listed in stdin in a terminal.

## Installing
To install it, execute install.sh in the project root.

## Dependencies
- w3m
- ImageMagick
- ncurses

## Color legend
Red - 

## Example usage

```sh
# Look for all png and jpg files in the current directory tree and print them
fd --type f '\.(png|jpe?g)$' | list-img

# Print all images in the current dir
ls | list-img

# Get all png images in the current directory and print them
ls | grep '\.png' | sort -R | list-img
```
## License
 © Grzegorz Kociołek 2020  
 GPLv3
