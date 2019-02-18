# 4. Managing Assets

## Overview

With LiveSYNC, you can present content to other people using a common big screen device. This can be for example a TV or a projector. The view of the control device can be mirrored to the big screen for example via an HDMI cable. In this case, it is clear that the presentation's content must be copied to the control device before the presentation begins.

However, LiveSYNC allows presenting content also to an audience that is using personal viewing devices. The number of viewing devices varies. It could be 4, 25, 110 or 1302. You may wonder where the content comes from in this case. Is it streamed from the control device to all of the audience devices? Is it streamed from a network server? Or is it played from local file copies on each device? LiveSYNC already supports more than one option. In most cases, the recommended solution is to use local file copies. These are called *assets*.

In this chapter, we will go through various methods and strategies for managing your assets. The assets include for example 360-degree photos and videos, ordinary 2D slides and videos, and custom hotspot icons. A presentation often uses a mix of them. Different presentations may use partially the same assets, partially different. LiveSYNC allows uses a central repository for all assets. You don't need to create multiple copies of large video files.

First, we will discuss different strategies. This will explain the basic concepts and answer *why* LiveSYNC is built as it is. 

!!! tip
    If you just need to quickly learn where to put your files, continue reading from [here](asset_management.md#where-should-my-files-go).

## Concepts

### Single File vs. Multi File

Every software product that supports embedding images, videos, and sound tracks must choose a strategy for handling external multimedia content. As an example, you can embed images into PowerPoint presentations and PDF files. The output will be a single file - often multiple megabytes in size. When you create a slightly different version, you'll get another large file. Their strategy is to embed all the content into a single file. It is easy to manage, but multiple variants quickly add up on your disk. 

Smart presentation application with focus on video content chooses a different strategy. This is almost mandatory, as video files tend to be *very* large and become unmanageable if stored as a single file.

!!! example
    FAT32 file system is often used on hard disks, USB flash drives, and memory cards. The total size of the drive could be as large as 2 TB (two terabytes), enough for 80 hours of 4K video captured with an iPhone. However, the size of each *individual file* may not exceed 4 GB (four gigabytes). If a single file strategy would be used, a presentation that combines multiple high-resolution 360-degree videos could be impossible to save on FAT32 file system!

It is a common practise to reuse material from previous presentations. In fact, a good speaker tries to adapt his presentation to his audience. Smart presentation application uses a strategy that supports combining content in different ways. This must happen without creating new copies of the source files every time.

!!! example
    A low-cost 16 GB tablet might have only about 10 GB available for user files. As a consequence, just a few variants of the same video presentation might fill its internal memory completely. Yet, majority of the bytes *inside* those files would be exactly the same. What a waste!

Sometimes, a large number of devices is used in a presentation. The time required to copy the files grows exponentially along the file size and number of devices. Smart presentation application allows copying *only* the changed files when it is necessary to update content.

!!! example 
    Imagine a situation, where you have copied 3 GB of content to 40 VR headsets. (That will take hours, by the way.) Then, your boss says that one logo image must be changed. A single file strategy would mean copying again 120 GB of data simply to update a tiny 1 kB logo file to all devices.

All in all, for a smart presentation application with a focus on video, there is really only one feasible strategy: multi file. Hence, in LiveSYNC the assets must be stored on each device as individual files.

### Central Media Repository

It is logical to create *a central media repository* where the content files will be copied to. The application does not need to crawl through the whole file system to find new files. Presentations consist of of combinations of files in the repository. A project file becomes very light-weight, as it only references to the multimedia files. The number of presentation variants is almost unlimited. And, updating a single file is as quick and easy as it should be.

## Which Files Must Be Copied?

### Photos

### Videos

### Slides

### Icons

## Where Should My Files Go?

### iOS

**On iOS, LiveSYNC uses the app's own file sharing folder as its central media repository**. The device might contain plenty of other photo and video content. The presenter may not want all of them to appear in the presentation tool. Hence, it is better to use a separate location.

Yet, the presenter may have wish to present content for example from the device's own photo or video repository. This is also possible with LiveSYNC. For example, contents of your iPad's *Camera Roll* appear as a subfolder.

### Android

**On Android, LiveSYNC uses a subfolder */Movies/LiveSYNC* in the public area of the device's internal memory as its central media repository**. This allows easy file copying back and forth, as well as sharing files with other apps.

In case you have a device that supports a memory card (SD card), the media files can be copied there, too. The logical path will be the same ie. */Movies/LiveSYNC* is searched also from the SD card. In case you have same filename in both directories, the internal memory has a precedence.

### Oculus

**On Oculus, LiveSYNC uses a subfolder */Movies/LiveSYNC* in the public area of the device's internal memory as its central media repository**. This allows easy file copying back and forth, as well as sharing files with other apps.

In case you have a GearVR compatible phone that supports a memory card (SD card), the media files can be copied there, too. The logical path will be the same ie. */Movies/LiveSYNC* is searched also from the SD card. In case you have same filename in both directories, the internal memory has a precedence.

## How To Copy Files?

### iOS
1. Download [iTunes](https://www.apple.com/itunes/download/).
2. Connect the included USB 2.0 cable to your computer and iPad.
3. Select device from iTunes on your computer.
4. Select Apps/File Sharing.
5. Select LiveSYNC.
6. Click and drag files and folders to LiveSYNC Documents.
7. Open LiveSYNC on iPad -> Select channel number -> Player -> and pull to refresh contents on the left side (where demo contents are located).

Take a look at our [video tutorial](https://vimeo.com/222670351) to see how files are copied. After adding video, image, and .png hotspot files to LiveSYNC pull-to-refresh and update contents of LiveSYNC.

If you wish to transfer files between your Mac computer and your Android device/s you need to install an app called [Android File Transfer](https://www.android.com/filetransfer/).  

### Android

### Oculus

## Common Strategies

### Content Folder

### USB Memory

### DropBox
