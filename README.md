# Video diet

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg?label=license)](https://www.gnu.org/licenses/gpl-3.0) [![Last commit](https://img.shields.io/github/last-commit/hiancdtrsnm/video-diet.svg?style=flat)](https://github.com/hiancdtrsnm/video-diet/commits) [![GitHub commit activity](https://img.shields.io/github/commit-activity/m/hiancdtrsnm/video-diet)](https://github.com/hiancdtrsnm/video-diet/commits) [![Github Stars](https://img.shields.io/github/stars/hiancdtrsnm/video-diet?style=flat&logo=github)](https://github.com/hiancdtrsnm/video-diet) [![Github Forks](https://img.shields.io/github/forks/hiancdtrsnm/video-diet?style=flat&logo=github)](https://github.com/hiancdtrsnm/video-diet) [![Github Watchers](https://img.shields.io/github/watchers/hiancdtrsnm/video-diet?style=flat&logo=github)](https://github.com/hiancdtrsnm/video-diet) [![GitHub contributors](https://img.shields.io/github/contributors/hiancdtrsnm/video-diet)](https://github.com/hiancdtrsnm/video-diet/graphs/contributors)

This project aims to reduce the spaces of your videos encoding it on `hevc`.

## Why video-diet?
The answer is easy. I have a lot old-movies/videos taking a lot of space in the hard-drive.
So I'm always short on disk space, the by accident discover de `hevc` codec. when i need to shrink a video of `3GB`
to upload it to `Telegram`, the convertion take my 3GB movie and returned a 300 MB with the same quality 😱. So I
decided that I would convert all my video files, but they are a lot, so I build this tool for it.

More info about `hevc`:

https://en.wikipedia.org/wiki/High_Efficiency_Video_Coding


## Installation

<div class="termy">

```console
$ pip install video-diet
```

</div>

## Example

### For a file

```bash
video-diet file --path test.mp4
```
This option conserve the original file

## For a folder
```bash
video-diet folder --path ~/Videos
```
This option replaces the original file for the converted files

## Note

The video conversion can take some time. Depending on the original video properties; the conversion time can be longer than the video.

## For developers

### You must first install *poetry*

Poetry provides a custom installer that will install `poetry` isolated from the rest of your system by vendorizing its dependencies. This is the recommended way of installing `poetry`.

**osx / linux / bashonwindows install instructions**

`curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python`

**windows powershell install instructions**

`(Invoke-WebRequest -Uri https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py -UseBasicParsing).Content | python`

The installer installs the `poetry` tool to Poetry's `bin` directory. On Unix it is located at `$HOME/.poetry/bin` and on Windows at `%USERPROFILE%\.poetry\bin`.

This directory will be in your `$PATH` environment variable, which means you can run them from the shell without further configuration.

### Then you need to configure the environment

Inside the project make `poetry install` and after `poetry shell` for start the virtualenv.

For testing the code run `video-diet`.

See [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

Good luck 😉.

Project Structure based on awesome tutorial by @tiangolo at https://typer.tiangolo.com/tutorial/package

https://ffmpeg.org/download.html
