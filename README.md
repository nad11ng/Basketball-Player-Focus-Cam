# Basketball Player Focus Cam

A computer vision project for segmenting and tracking basketball players in short match videos and generating automatic focus cameras for individual players.

## Project Goal

The goal is to create a visualization that combines:

- The original video with colored segmentation masks.
- Object IDs for tracked players.
- Individual camera crops that automatically follow selected players.

## Planned Features

- Read a basketball video and extract frames.
- Segment selected players.
- Track players across video frames.
- Generate smooth focus-camera crops.
- Display multiple focus cameras in a grid.
- Export the resulting videos.

## Project Structure

```text
basketball-player-focus-cam/
├── data/
│   ├── raw/
│   └── frames/
├── checkpoints/
├── outputs/
├── notebooks/
├── docs/
├── src/
│   ├── __init__.py
│   ├── config.py
│   ├── main.py
│   ├── video_utils.py
│   ├── segmenter.py
│   ├── focus_cam.py
│   └── visualizer.py
├── .gitignore
├── requirements.txt
└── README.md
```

## Setup

Create and activate a virtual environment on Windows:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install the basic dependencies:

```powershell
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Model-specific dependencies will be added after the segmentation and tracking approach has been selected.

## Development Status

Initial project setup.

Segmentation, tracking, and focus-camera generation are not implemented yet. The model and execution environment have not been finalized.

## Initial Prototype

The first prototype will process a short video with one continuous camera shot and follow one selected player. Multi-player tracking and a focus-camera grid will be added afterward.