# Flash Attention Builder

This repository builds flash-attention wheels for various CUDA and PyTorch combinations from the official [Dao-AILab/flash-attention](https://github.com/Dao-AILab/flash-attention) repository.

## Features

- Builds from official flash-attention repository
- Supports multiple CUDA versions: 11.8, 12.1, 12.2, 12.3, 12.4, 12.5, 12.6, 12.8
- Supports multiple PyTorch versions: 2.0.1 through 2.7.0
- Supports Python 3.9 through 3.12
- Builds for both Windows and Linux
- Automatically uploads to GitHub releases

## Usage

1. Go to **Actions** tab
2. Select "Build flash-attention Wheels from Official Repo"
3. Click "Run workflow"
4. Enter the flash-attention version tag (e.g., `v2.6.3`)
5. Click "Run workflow"

## Testing

Use the "Test Flash Attention Build (Small Matrix)" workflow to test the build process with a minimal matrix before running the full build.

## Built Wheels

Pre-built wheels are available in the [Releases](https://github.com/tuankiet2s/flash-attention-builder/releases) section.

## Source

Built from: https://github.com/Dao-AILab/flash-attention 