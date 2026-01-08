# tagr

A simple command-line interface for editing metadata tags on FLAC and Ogg Vorbis audio files.

## Requirements

- `metaflac` (from the `flac` package)
- `vorbiscomment` (from the `vorbis-tools` package)

On Debian/Ubuntu:
```
sudo apt install flac vorbis-tools
```

On Arch:
```
sudo pacman -S flac vorbis-tools
```

## Usage

```
tagr [-r|-R] [directory]
```

If no directory is specified, the current directory is used.

### Options

- `-r`, `-R` - Recurse into subdirectories
- `-h` - Show help message

### Interactive Commands

Once running, tagr displays the current tags for each file and accepts the following commands:

- `1-8` - Edit a tag by number (TITLE, ARTIST, ALBUM, ALBUMARTIST, DATE, TRACKNUMBER, GENRE, COMMENT)
- `a` - Add a custom tag
- `d` - Delete a tag
- `n` - Skip to next file
- `q` - Quit

## License

This project is released into the public domain under the Unlicense. See UNLICENSE for details.
