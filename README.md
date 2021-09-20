# Podcaster
Podcaster is a short shell script that takes one or more youtube urls, then reduces the bitrate and concatenates them in a single file.

It is a convinient tool when memory is limited, since audio quality in podcasts (or ttrpgs) doesn't play an important role, as long as it has a minimum bitrate.

## Dependencies
Podcaster depends on ffmpeg and youtube-dl.

## Usage
```
    sh podcaster <youtube url> [further youtube urls] [-b=BITRATE] [-o=OUTPUT_NAME]
```
    - `BITRATE`: expects a ffmpeg format, i.e. "120k" for 120 kbps. The default bitrate at the output is currently 50 kbps.
    - `OUTPUT_NAME`: the name of the final file **without** the extension. By default it's value is `out` so the resulting file is `out.mp3`.
