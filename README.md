# IMPORTANT: Bug Fixes

## your can find full article here
https://hackthestuff.com/article/how-to-face-detection-using-webcam-in-php

## `navigator.getUserMedia`

`navigator.getUserMedia` is now deprecated and is replaced by `navigator.getUserMedia`. To fix this bug replace all versions of `navigator.mediaDevices.getUserMedia` with `navigator.mediaDevices.getUserMedia`

## Low-end Devices Bug

The video eventListener for `play` fires up too early on low-end machines, before the video is fully loaded, which causes errors to pop up from the Face API and terminates the script (tested on Debian [Firefox] and Windows [Chrome, Firefox]). Replaced by `playing` event, which fires up when the media has enough data to start playing.
