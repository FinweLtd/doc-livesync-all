# 4. Managing Assets

## Overview

With LiveSYNC, you can present various kinds of content to other people. Before your presentation, the content files must be manually copied to specific locations. This way LiveSYNC can find and access them during the presentation.
 
 The content files are called *assets*. In this chapter, we will go through various methods and strategies for managing your assets.

!!! tip
    LiveSYNC contains free content samples. These are bundled with the app. You can study and evaluate the app using demo content. Return here when you want to learn how to present your own files.

### Strategy

Every software product that supports embedding images, videos, and sound tracks must choose a strategy for handling multimedia files. This decision is fundamental. The chosen strategy defines how easy it is to manage your project with that application. For example, to share a finished work, store multiple versions of it, or to make some last-minute modifications.

You have probably created presentations using *PowerPoint* or *Keynote* application. These tools make adding images easy. Have you ever though about what happens in the background when you drag an image onto a slide? When you save the presentation, the output will be a single file. This file contains *everything* that belongs to your presentation, including all the images. A single file is easy to manage on disk and share via email. However, as everything is embedded file size can easily grow to several megabytes. Sometimes, tens of megabytes. What would happen if you added a couple of high-resolution videos? 

Single-file strategy becomes unpractical when the file size becomes too large. Hence, applications that make extensive use of video content typically choose a different strategy. The project is not stored as a single file that contains everything. Instead, all multimedia files are stored as individual files. A light-weight project file *references* to them - it does not embed them. This approach has many benefits, but also one drawback: a project becomes partially broken if any of the referenced files is not present. Hence, moving the files around or renaming them frequently should be avoided. 

Also **LiveSYNC uses this approach: a presentation consists of multiple smaller files. Not just one huge file**. Remember to copy all the files that you need in your presentation.

### File System Limitations

To avoid common pitfalls when dealing with large video files as part of presentations, we need to understand some technical and practical limitations. Some of them comes from the *file system*.

All the assets that belong to a presentation must be stored as files on a mass storage device. This might be the hard drive of the computer where you edit the files. Or, the internal mass memory of the tablet you use for presentations. Or, a USB memory stick that you use for quickly copying files to multiple VR headsets. Or, an SD card that you use for expanding your Android tablet's storage capacity. All these devices use a file system for managing the files. It defines how the total size of the mass memory is divided into smaller blocks, and how these blocks are allocated for individual files. 

A file system also sets two important hard limits. One of them is the total number of bytes it can store ie. max drive size in bytes. Another is the maximum number of bytes that a single file can reserve ie. max file size in bytes. After all other files, your mass storage device must have enough free space to store your presentation files (their total size). And, each of your files must not exceed the file system's max file size limit.

!!! example
    Jean has purchased a cheap Android tablet. It has 16 GB internal storage capacity. However, Android operating system and bundled factory apps (which cannot be removed) consume 6 GB. Other apps and Jean's photos, music, video clips, and web browser cache consume another 4 GB. Jean has only 6 GB left. The total size of all the files she needs in her presentation must not exceed 6 GB. Else, she will need to clean up her tablet to release some memory.

!!! example
    Jean has bought a 16 GB SD card to expand the storage capacity of her Android tablet. The SD card is formatted with FAT32 file system. FAT32 is often used on older hard disks, USB flash drives, and memory cards. It is fairly well supported on different devices. The total size of a FAT32 formatted drive could be as large as 8 TB (eight terabytes), enough for 300 hours of 4K video captured with an iPhone. However, the size of each *individual file* may not exceed 4 GB (four gigabytes). After adding the SD card, Jean has 16 GB for her presentation files (and 6 GB free on her tablet's internal memory). However, each of her video files must stay below the 4 GB limit.
    
!!! example
    One of Jean's videos is 5.6 GB. It is a high-resolution video that she wishes to present using an Oculus Go headset. She plans to control the presentation with her Android tablet. Jean has a few options for overcoming her SD card's 4 GB max file size limitation:
       
    a) She can try to format her SD card with exFAT file system. If her tablet recognizes the card, the problem is solved. exFAT is a newer file system and has *much* larger limits. 5.6 GB file will work easily.
    
    b) She can make space on her tablet's internal memory and copy the file there. That drive is very likely formatted with a different file system and does not have the 4 GB limit.

    c) She can encode a low-resolution version of the video and use that in her tablet. She can still use the high-resolution version on her Oculus Go headset. The filenames must match, so that LiveSYNC can identify them as the same video.

!!! tip
    On iOS devices, you cannot expand the storage capacity with an SD card. When you are purchasing a new iPhone or iPad, invest in a model that has enough storage space for your needs.
    
    On *some* Android devices, you can use an SD card for expanding the storage capacity. When you are purchasing a new Android phone or tablet, check if it supports an SD card. If not, choose another model or invest in a model that has enough built-in storage capacity.
    
!!! tip
    If you have videos that are larger than 4 GB, you may encounter problems in storing or transferring them. However, usually such problems can be solved. You might be able to reformat the storage device with another file system type (such as exFAT). Beware that formatting destroys all the data! If you are transferring files, try another device memory stick or SD card. Or, try transferring the files via network connection.

### Redundancy

When you create a slightly different version, you'll get another large file. Their strategy is to embed all the content into a single file. , but multiple variants quickly add up on your disk. 


It is a common practise to reuse material from previous presentations. In fact, a good speaker tries to adapt his presentation to his audience. Smart presentation application uses a strategy that supports combining content in different ways. This must happen without creating new copies of the source files every time.


Sometimes, a large number of devices is used in a presentation. The time required to copy the files grows exponentially along the file size and number of devices. Smart presentation application allows copying *only* the changed files when it is necessary to update content.

!!! example 
    Imagine a situation, where you have copied 3 GB of content to 40 VR headsets. (That will take hours, by the way.) Then, your boss says that one logo image must be changed. A single file strategy would mean copying again 120 GB of data simply to update a tiny 1 kB logo file to all devices.

All in all, for a smart presentation application with a focus on video, there is really only one feasible strategy: multi file. Hence, in LiveSYNC the assets must be stored on each device as individual files.

### Central Media Repository

It is logical to create *a central media repository* where the content files will be copied to. The application does not need to crawl through the whole file system to find new files. Presentations consist of of combinations of files in the repository. A project file becomes very light-weight, as it only references to the multimedia files. The number of presentation variants is almost unlimited. And, updating a single file is as quick and easy as it should be.

### Assets

In short, the presentation's assets are the files that you will need in your presentation. They include for example:

- 360-degree photos
- 360-degree videos
- Ordinary 2D photos
- Ordinary 2D videos
- Slide images
- Custom tag and hotspot icons
- Video stream configuration files
- Project files

![Enterprise feature](../img/enterprise_feature.png)

- 2D map images
- 3D map models
- Camera path files

Typically, a presentation combines several kinds if assets. They can be partially the same with other presentations, and partially different.

### Big Screen

You can use a common big screen device for showing content to an audience. This can be for example a TV or a projector. **When you present content via big screen, you need to copy your presentation's assets to the control device. There is no need to copy them anywhere else.** This is because the view from your control device is mirrored to the big screen as a video stream, not as command messages. For example, you can connect an iPad to a TV using a standard HDMI cable (you will also need an adapter from Apple).

!!! note
    Some modern TVs and projectors support playing photos and videos from a USB memory stick. You may wonder if that approach can be used for showing also 360-degree content. Technically, the photos and videos can be played. However, current display devices do not understand the special projections that are used for storing 360-degree content. In addition, they do not provide interactivity ie. ways for panning and zooming 360-degree content. Hence, this approach does not really work.

### Viewing Devices

LiveSYNC supports presenting content also via personal viewing devices. You may wonder where the content comes from in this case. Is it streamed from the control device to all of the audience devices? Is it streamed from a local server or a cloud service? Is it played from local file copies on each device? LiveSYNC already supports more than one option. 

In most cases, the recommended solution is to use local file copies. This is because streaming high-resolution video to a number of devices tends to congest local network connection. With local file copies, the user experience is great and you don't need to struggle with network bandwidth issues. This chapter focuses on local file copy approach. If you want to learn how to use streaming with LiveSYNC, you can read about it [here](streaming.md).

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
