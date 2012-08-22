FFCameraSample uses the native camera API to record video. However instead of using the platform encoder to write to an MP4 file, this app will use FFmpeg to write out to an MPEG-2 file. This app currently only records video and not audio. While recording, the video file will be read, decoded and displayed on the screen.

The FFmpeg related functionality is provided through [libffbb](https://github.com/hardisonbrewing/libffbb) which has been copied into the `src` directory. See libffbb for instructions on building FFmpeg.

Demo Video:  
This was the initial demo video. The playback lag should be fixed.  
[http://www.youtube.com/watch?v=baOL5EJrJ9U](http://www.youtube.com/watch?v=baOL5EJrJ9U)

Related support forum post:  
[Camera API NV12 frame to AVFrame (FFmpeg)](http://supportforums.blackberry.com/t5/Native-Development/Camera-API-NV12-frame-to-AVFrame-FFmpeg/td-p/1842089)

Built using the 10.0.6 BlackBerry 10 NDK, and tested on the BlackBerry Dev Alpha device.