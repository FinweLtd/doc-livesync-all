

## 360-degree Content

360 video is video that’s recorded from all angles using a special rig of multiple cameras, or one camera with multiple lenses. The viewer can navigate around based on their central point in space, dictated by the camera.

#### Monoscopic

Monoscopic (Mono) video, this is the most common type of 360 videos which is captured using a single lens system from a single point of view. The end result of a monoscopic 360 video viewed through a VR headset is that everything appears the exact same distance away. 

#### Stereoscopic

Stereoscopic( Stereo) video is captured using a twin lens system, which makes it the “3D” type of 360 video. Stereo videos are recorded side by side with a separate recording mapped to each eye. The end result of a stereoscopic 360 video viewed through a VR headset is that some objects appear closer than others, simulating our own binocular vision. 

## 180-degree Content

#### Monoscopic

#### Stereoscopic

## 2D Content

#### Monoscopic

#### Stereoscopic

## Resolution

LiveSYNC uses media player on the back-end and that limits the resolution when it comes to playable video files. Any video that plays with the device's own video player should also work with LiveSYNC.
Choosing the right resolution and encoding is the key to an excellent experience. 

We advise using .mp4 format video files with resolution 1920x960 or 3840x1920 since these are best supported across devices. However, only 4k capable devices will play 3840x1920. We recommend one can get better balance by targeting a bitrate somewhere between 30-60 Mbps. 

If you have a mix of older and newer devices, it is much safer to use 3840x1920 for 4k capable devices and for old devices 1920x960
by using the same file name for the same video content with different resolutions. 

We have built support for Facebook 360 audio (.tbe files). This has not yet been released for all platforms but it is available on request for example for GearVR.

The maximum resolution depends on each device's hardware capabilities. Notice that offline video files need to be copied for each device during the setup phase, and this opens a possibility to use a different resolution (but same filename) variants on different devices, in order to get the best possible quality on each platform.


### iOS supported video format

- H.264 video up to 720p, 30 frames per second, Main Profile level 3.1 with AAC-LC audio up to 160 Kbps, 48kHz, stereo audio in .m4v, .mp4, and .mov file formats;

- MPEG-4 video, up to 2.5 Mbps, 640 by 480 pixels, 30 frames per second, Simple Profile with AAC-LC audio up to 160 Kbps per channel, 48kHz, stereo audio in .m4v, .mp4, and .mov file formats;

- Motion JPEG (M-JPEG) up to 35 Mbps, 1280 by 720 pixels, 30 frames per second, audio in ulaw, PCM stereo audio in .avi file format.

- Max size: 100 MB

### Android Supported Video Format

|              | SD (Low quality) | SD (High quality) | SD (High quality) |
| ------------ | ------------- | ------------ |------------ |
| Video codec | H.264 Baseline Profile  | 	H.264 Baseline Profile	 |H.264 Baseline Profile |
| Video resolution | 176 x 144 px | 480 x 360 px | 1280 x 720 px |
| Video frame rate | 12 fps  | 30 fps | 30 fps |
| Video bitrate | 56 Kbps  | 500 Kbps | 2 Mbps |
| Audio codec | AAC-LC | AAC-LC | AAC-LC |
| Audio channels | 1 (mono) | 2 (stereo) | 2 (stereo) |
| Audio bitrate | 24 Kbps  | 128 Kbps | 92 Kbps |


- For 3GPP and MPEG-4 containers, the moov atom must precede any mdat atoms, but must succeed the ftyp atom.

- For 3GPP, MPEG-4, and WebM containers, audio and video samples corresponding to the same time offset may be no more than 500 KB apart. To minimize this audio/video drift, consider interleaving audio and video in smaller chunk sizes.

- Max size: 100 MB

!!! tip
    
    If some of your devices do not support 4K video (3840x1920), you can copy there a lower quality variant (1920x960). 
    
 
## Encoding a video
 
 Video encoding is the process of preparing the video for output, where the digital video is encoded to meet proper formats and specifications. In other words, video encoding is the process of converting digital video files from one format to another. 
 
  If you are not sure with which resolution to use, try to play the video you want to use for the presentation on the devices you're using. If it plays then it likely is supported by LiveSYNC. If you wish to encode video, we have prepared a [tutorial](..//articles/video_encoding.md) on how to encode a video using an open source software (HandBrake). 

## File Naming Conventions

LiveSYNC supports both Over-Under and Side-by-Side formats for video files. The only thing you need to do is add the following prefix to the video file:

- _3DOU.mp4 

- _3SBS.mp4 

- _3DTB.mp4 

- _3DBT.mp4 

So for example if your file name is myvideo.mp4, you just need to modify the filename to myvideo_3DOU.mp4. 

!!! Note

    If your own content files do not work:
 
       - Make sure to use .mp4 format videos, .jpg format photos, and .png format hotspot images.
       
### Does LiveSYNC support stereoscopic content?

We have stereoscopic 360 content support already built for equirectangular panoramas (the usual equirectangular configurations over-under and side-by-side), but it hasn't been released yet officially. This will be included in the next release that is coming within a few weeks of time. However, if you are in a hurry we may be able to provide a custom build earlier.


### Does LiveSYNC support cubemap projection?

Currently, no. We have supported cubemap projection in some apps earlier and if there is demand for it, we will definitely add it to LiveSYNC as well. But with the current version, you'll have to export the images in an equirectangular format or convert your existing cubemaps to equirectangular.

