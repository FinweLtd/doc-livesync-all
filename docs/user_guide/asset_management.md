# 4. Managing Assets

## Basics

With LiveSYNC, you can present various kinds of content to other people. Before your presentation, the content files must be manually copied to specific locations. This way LiveSYNC can find and access them during the presentation.
 
 The content files are called *assets*. In this chapter, we will go through various methods and strategies for managing your assets.

!!! tip
    LiveSYNC contains free content samples. These are bundled with the app. You can study and evaluate the app using the demo content. Return here when you want to learn how to present your own files.

### File Storage Strategy

Every software product that supports embedding images, videos, and sound tracks must choose a strategy for handling multimedia files. This decision is fundamental. The chosen strategy defines how easy it is to manage your project with that application. For example, to share a finished work, store multiple versions of it, or to make some last-minute modifications.

You have probably created presentations using *PowerPoint* or *Keynote* application. These tools make adding images easy. Have you ever though about what happens in the background when you drag an image onto a slide? When you save the presentation, the output will be a single file. This file contains *everything* that belongs to your presentation, including all the images. A single file is easy to manage on disk and share via email. However, as everything is embedded file size can easily grow to several megabytes. Sometimes, tens of megabytes. What would happen if you added a couple of high-resolution videos? 

Single-file strategy becomes unpractical when the file size becomes too large. Hence, applications that make extensive use of video content typically choose a different strategy. The project is not stored as a single file that contains everything. Instead, all multimedia files are stored as individual files. A light-weight project file *references* to them - it does not embed them. This approach has many benefits, but also one drawback: a project becomes partially broken if any of the referenced files is not present. Hence, moving the files around or renaming them frequently should be avoided. Also **LiveSYNC uses this approach: a presentation consists of multiple smaller files. Not just one huge file**.

### File System Limitations

To avoid common pitfalls when dealing with large video files in presentations, we need to understand technical and practical limitations. Some of them come from the *file system*.

All the assets that belong to a presentation must be stored as files on a mass storage device. This might be the hard drive of the computer where you edit the files. Or, the internal mass memory of the tablet you use for presentations. Or, a USB memory stick that you use for quickly copying files to multiple VR headsets. Or, an SD card that you use for expanding your Android tablet's storage capacity. All these devices use a file system for managing the files. It defines how the total size of the mass memory is divided into smaller blocks, and how these blocks are allocated for individual files. 

The type of the file system sets some important hard limits. One of them is the total number of bytes that a drive can store ie. *max volume size in bytes*. This is rarely a bottleneck nowadays as theoretical limits are far higher than current storage capacities. Another limitation is the maximum size that a single file can be ie. *max file size in bytes*. This is important when you deal with large video files. **None of your files can exceed the file system's max file size limit.** Often you encounter problems with files that are over 4 GB in size. Another common problem is that the presentation device simply does not have enough free space for the presentation's files.

!!! example
    Jean has purchased a cheap Android tablet. It has 16 GB internal storage capacity. However, Android operating system and bundled factory apps (which cannot be removed) consume 6 GB. Other apps and Jean's photos, music, video clips, and web browser cache consume another 4 GB. Jean has only 6 GB left. Thus, the total size of all the files she needs in her presentation must not exceed 6 GB. Else, she will need to clean up her tablet to release some memory. Jean regrets not buying a 32 GB model.
    
    Based on a tip from her friend, Jean buys a 16 GB SD card to expand the storage capacity of her Android tablet. The SD card is formatted with FAT32 file system. FAT32 is often used on older hard disks, USB flash drives, and memory cards. It is fairly well supported on different devices. The theoretical size of a FAT32 formatted drive could be as large as 8 TB (eight terabytes). Enough for 300 hours of 4K video captured with an iPhone. However, the size of each *individual file* may not exceed 4 GB (four gigabytes). That is only 10 minutes of 4K video captured with an iPhone. After adding the SD card, Jean has 16 GB more storage space.

    Each of her video files must stay below the 4 GB limit. However, one of Jean's videos is 6.5 GB. It is a high-resolution video that she wishes to present using an Oculus Go headset. She plans to control the presentation with her Android tablet. Jean has several options for overcoming her SD card's 4 GB max file size limitation:
       
    a) She can try to format her SD card with exFAT file system. If her tablet recognizes the card, the problem is solved. exFAT is a newer file system and has *much* larger limits. 6.5 GB file will work easily.
    
    b) She can make space on her tablet's internal memory and copy the file there instead. That drive is very likely formatted with a different file system and does not have the 4 GB limit.

    c) She can encode a smaller version (low resolution / bitrate) version of the video and use that in her tablet. She can still use the high-resolution version on her Oculus Go headset. The filenames must match, so that LiveSYNC can identify them as the same video.
    
    d) She can use a video editor application to split her video to shorter clips, each below the 4GB limit. During the presentation, she will simply start the next clip when the previous one ends.

!!! tip
    On iOS devices, you cannot expand the storage capacity with an SD card. There are memory sticks intended for iOS devices, but they only work with the manufacturer's own app - not LiveSYNC. Hence, when you are purchasing a new iPhone or iPad, invest in a model that has enough built-in storage space for your needs. 
    
    On *some* Android devices, you can use an SD card for expanding the storage capacity. When you are purchasing a new Android phone or tablet, check if it supports an SD card. If not, choose another model or invest in a model that has enough built-in storage capacity.
    
    We recommend purchasing a device that has at least 32 GBs of internal storage space.
    
!!! tip
    If you have videos that are larger than 4 GB, you may encounter problems in storing or transferring them. However, usually such problems can be solved. You might be able to simply reformat the storage device with another file system type (such as exFAT). Beware that formatting destroys all the data! 
    
    Using a different device for storing or transferring the files often helps. You can also try transferring the files via cable or via network connection.
    
    If nothing else helps, consider splitting a large file to multiple smaller ones (multiple video clips). Or, encode your video again to lower resolution and lower bitrate to create a smaller file.

### Dealing With Redundancy

Video files consume a lot of storage space. Thus, it is important to **learn to fight against unintended redundancy**. Don't get this wrong: creating a backup is always a good idea. That is intended redundancy. However, when you are busy preparing for a presentation, it is easy to forget that you have one version of a video clip here and another there. Files that consume hundreds of megabytes or even multiple gigabytes each quickly add up. And cleaning is laborious!

One strategy is to create a new folder on your computer. This folder will be the *master directory* of your presentation. It should contain all the necessary assets and nothing else. Keep it tidy: delete old and extra versions immediately. Create backups by copying the whole folder e.g. to an external drive. Delete old content on your presentation devices and copy there the contents of your master directory as-is. The idea is to focus on this one presentation and keep its assets in one directory. This approach works well if you use shared devices that must be cleared frequently.

The approach described above is not suitable for all cases. Some users have presentations often and reuse material from previous presentations. Creating a new presentation folder every time would mean redundant copies of the same files. Another strategy is to create one master directory and a number of subfolders. Folder titles can be for example dates or topics, whatever suits your situation. You will quickly get familiar with your own content archive. During a presentation, you can adapt to the audience as you go and present content directly from your content archive. Maintain a backup of the whole archive on an external drive, and copy new files to your presentation devices incrementally. This approach works well if you have a set of devices reserved for your own use.

A third option is a hybrid one. You will build a content archive as explained above. And, sometimes create a subfolder for a particular presentation by copying the necessary assets there. This means that there will be multiple copies of some of the files but only for a while. After the presentation, you can simply delete its folder - all of its assets are already in your archive folders, too.

!!! note
    To keep the user interface simple, **LiveSYNC supports only one level of subdirectories**. We encourage you to make use of them. Choose one strategy for organizing your content, and stick to it.

### Transfer Times

Sometimes, a large number of devices is used in a presentation. It is good to remember that **the time required to copy the files grows exponentially along the total file size and the number of devices** - unless you can do it in parallel using multiple copy stations. Nevertheless, you should have the final version ready early enough so that there is enough time to copy the assets in place.

Notice that last-minute changes can be problematic. Changing even one small icon requires going through all the devices again. Moreover, on iOS devices you may have to copy the whole folder again even if you need to change a single file inside it. This is because Apple's *iTunes* application, which is used for copying files for iOS devices, has very limited file management capabilities.

!!! example 
    Lisa is a teacher in elementary school. They have a rack of 20 iPads, which any of the teachers can reserve for their class. Lisa is preparing a presentation for the parent's night. Her students have made a 360-degree video of their day at school. She plans to use the iPads to show the video to the parents. Lisa has a single presentation folder that contains one 3 GB video file and a few 360-degree photographs. Her students copied the files to all iPads. Suddenly Liza realizes that their 360-degree group photo is missing.
    
    If Lisa adds the missing photo to her presentation folder, she must copy the whole folder again. This is because of limitations in Apple's iTunes application. She quickly calculates that copying 3 GB * 20 devices means 60 GB in total. That will take hours. Lisa decides to create another folder that contains only this one image. Since the image is just 5 MB in size, Lisa needs to copy 5 MB * 20 devices = 100 MB. She will be ready in 15 minutes.

### Central Media Repository

It is logical to create *a central media repository* where the content files will be copied to. The application does not need to crawl through the whole file system to find new files. Presentations consist of combinations of files in the repository. A project file becomes very light-weight, as it only references to the multimedia files. The number of presentation variants is almost unlimited. And, updating a single file is as quick and easy as it should be.

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
