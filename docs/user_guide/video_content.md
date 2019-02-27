
## File Naming Conventions

### 360-degree Content

#### Monoscopic

#### Stereoscopic

### 180-degree Content

#### Monoscopic

#### Stereoscopic

### 2D Content

#### Monoscopic

#### Stereoscopic

### Resolution

### Encoding a video

LiveSYNC uses media player on the back-end and that limits the resolution when it comes to playable video files. Any video that plays with the device's own video player should also work with LiveSYNC.
Choosing the right resolution and encoding is the key to an excellent experience. 

We advise using .mp4 format video files with resolution 1920x960 or 3840x1920 since these are best supported across devices. However, only 4k capable devices will play 3840x1920. We recommend one can get better balance by targeting a bitrate somewhere between 30-60 Mbps. 

If you have a mix of older and newer devices, it is much safer to use 3840x1920 for 4k capable devices and for old devices 1920x960
by using the same file name for the same video content with different resolutions. 

We have built support for Facebook 360 audio (.tbe files). This has not yet been released for all platforms but it is available on request for example for GearVR.

The maximum resolution depends on each device's hardware capabilities. Notice that offline video files need to be copied for each device during the setup phase, and this opens a possibility to use a different resolution (but same filename) variants on different devices, in order to get the best possible quality on each platform.


### Does LiveSYNC support stereoscopic content?

We have stereoscopic 360 content support already built for equirectangular panoramas (the usual equirectangular configurations over-under and side-by-side), but it hasn't been released yet officially. This will be included in the next release that is coming within a few weeks of time. However, if you are in a hurry we may be able to provide a custom build earlier.


### Does LiveSYNC support cubemap projection?

Currently, no. We have supported cubemap projection in some apps earlier and if there is demand for it, we will definitely add it to LiveSYNC as well. But with the current version, you'll have to export the images in an equirectangular format or convert your existing cubemaps to equirectangular.


!!! Note

    If your own content files do not work:
    
       - Make sure to use .mp4 format videos, .jpg format photos, and .png format hotspot images.
       - If some of your devices do not support 4K video (3840x1920), you can copy there a lower quality variant (1920x960). Photos will be automatically scaled to the device's maximum size.