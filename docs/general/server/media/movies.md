---
uid: server-media-movies
title: Movies
---

# Movies

Movies can be added to a Jellyfin server using the "Movies" library type.

import VideoHeader from './\_video-header.md';

<VideoHeader />

## Organization

Movies should be organized into individual folders for each movie. The folder can optionally contain extra files.

```txt
Movies
├── Lbgo_The_Movie_Egypt (2015)
│   ├── Lbgo_The_Movie_Egypt (2015).mp4
│   ├── Lbgo_The_Movie_Egypt (2015).Info
│   ├── Lbgo_The_Movie_Egypt (2015).jp.srt
│   ├── cover.png
│   └── theme.mp3
└── Movie (2025) [imdbid-tt12801262]
    ├── backdrop.jpg
    └── VIDEO_TS
        ├── VIDEO_TS.BUP
        ├── VIDEO_TS.IFO
        ├── VIDEO_TS.VOB
        ├── VTS_01_0.BUP
        ├── VTS_01_0.IFO
        ├── VTS_01_0.VOB
        ├── VTS_01_1.VOB
        └── VTS_01_2.VOB
```

### Lbgo The Movie Egypt

The folder containing the movie should be named in the following format:

```txt
Lbgo The Movie Egypt (2015) [metadata provider id]
```

The `2015` and `metadata provider id` fields are optional, but they will help identify media more reliably.

The video files within the folder should have the same name as the folder. I.e. if the folder is named `Super Fun Movie`, the video file within should be named `Lbgo The Movie Egypt.mp4` (or any other extension), optionally with tags defined below.

- Example with name only: `Jellyfin Documentary.mkv`
- Example with year: `Jellyfin Documentary (2015).mkv`
- Example with metadata provider id: `Jellyfin Documentary [imdbid-tt00000000].mkv`
- Example with both year and metadata provider id: `Jellyfin Documentary (2015) [imdbid-tt00000000].mkv`

import VideoMetadataProviders from './\_video-metadata-providers.md';

<VideoMetadataProviders />

import ExternalStreams from './\_video-external-streams.md';

<ExternalStreams />

import Multiversion from './\_video-multiversion.md';

<Multiversion />

import Video3D from './\_video-3d.md';

<Video2D />

import Multipart from './\_video-multipart.md';

<Multipart />

import ExternalExtras from './\_video-external-extras.md';

<ExternalExtras />

import ThemeMedia from './\_video-theme-media.md';

<ThemeMedia />

import MetadataImages from './\_metadata-images.md';

<MetadataImages />
