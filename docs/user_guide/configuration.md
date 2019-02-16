# 3. Configuration

## Channel Configuration

With LiveSYNC, you can present content to other people using a common big screen device and a set of personal viewing devices. In the latter case, the audience's viewing devices must be able to *communicate* with the presenter's control device. For example, the control device sends a command to change slide. The viewing devices respond that the slide was found and is now loaded on screen.

This communication takes place via *a wireless connection* that is opened between the control device and each viewing device. Before the connection can be opened, we must *configure* it for each device. For example, a device must know which role to adopt in the presentation, which connection type to use, and which channel number to join. In LiveSYNC, this is called *a channel configuration*. 

A set of devices that use the same connection type and the same channel number form *a device group*. They can exchange messages with each other. A device group is controlled by a single control device. This is the device that is configured to the director role. All other devices in the group must be configured to the audience role. Multiple device groups can operate in parallel even in the same room. Each group has its own control device.

Creating a channel configuration is a one-time operation. Whenever you start a presentation, you can re-use the same configuration. However, it is possible to create multiple channel configurations for each device. This is useful in dynamic environments, where multiple presentations take place simultaneously and device group sizes vary. On each device, only one connection can be open at a time.

Channel configuration is slightly different depending on the device's role (director or audience). Next, we will go through both cases.

### Director Role

#### iOS & Android

In a device group, one device must be configured to the director role. This device is typically an iPad or an Android tablet. The configuration is very similar on both platforms.

Follow the steps below to configure your device to the director role:

1. Start the LiveSYNC app. The *Home* screen appears. Initially, channel configurations do not exist. To create a new channel configuration, tap the big (+) button.

    ![Cover](img/config_android_director_step_1.jpg)

2. The *Setup* screen appears. First, tap the *Director* button to select the director role. Your selection is marked by underlining it, as in the image below. The selected role also appears in the setup progress menu on the left. Tap *Next* to proceed.

    ![Cover](img/config_android_director_step_2.jpg)

    !!! note
        Current setup page is underlined in the setup progress menu on the left. You can navigate through the setup pages by tapping the page titles in the progress menu, by swiping the page towards left or right, or by tapping the *Next* button on the bottom right corner. On Android, you can also use the device's *Back* button to return to previous page.
        
        Your input is validated on each page. You cannot proceed to the next page before your input is accepted. If you return to the first page and change the role, your input to the other pages is cleared.
        
        If you want to cancel channel configuration, tap the *Home* button on the top left corner and answer *OK* to the confirmation dialog that appears.

3. Other users can identify you by your LiveSYNC name. This can be for example your own name, a name that you have given to your device, or your device's model name. The name cannot be left empty. Its maximum length is 32 characters. Tap the text field to type a name. Tap *Next* to proceed.

    ![Cover](img/config_android_director_step_3.jpg)

4. Communication between the control device and the viewing devices is based on creating a wireless connection. The currently available connection types are listed. Choose a connection type that you wish to use. Notice that **the director device and the audience devices must use the same connection type**. Tap *Next* to proceed.

    ![Cover](img/config_android_director_step_4.jpg)

    !!! note
        A connection type that is supported by your device and your LiveSYNC software version may still be unavailable. If so, it is marked as *Not available* in the list. Tap the info button (i) next to it to learn why it is not available. As an example, you may need to enable Wifi or Bluetooth feature from the device's settings. Use pull-to-refresh gesture to update the list after fixing the issue.

5. Devices that are using the same connection type and the same LiveSYNC channel can exchange messages. Devices on a different channel will not see them. A random free channel number is given. If you want to get another one, tap the dice button next to the number. The channel numbers are in the range 1000-9999. Tap *Next* to proceed.

    ![Cover](img/config_android_director_step_5.jpg)

    !!! note
        You may wonder why the channel number is given randomly instead of asking it from the user. This is to prevent abuse. Consider a lesson in elementary school. Ms. Williams is about to begin a presentation and asks her students to join channel number 1234. However, young Mr. Smart Guy in the back seat configures his tablet *as the director* on that same channel. Now, other students' devices will form a connection randomly to one of the two competing control devices. Not being able input the channel number efficiently blocks such mischief.

6. Android only: a dialog appears to ask your permission to access the files on your device. Without a permission the LiveSYNC app cannot create the directory where your assets will go. Also, it cannot read from this directory even if you create it manually. Tap *Allow* to give file access permission.

    ![Cover](img/config_android_director_step_6.jpg)

7. The channel configuration is almost complete. This setup page reminds you that the presentation's assets must be copied to the device. This task will be covered in detail in the next chapter [Managing assets](asset_management.md). You can copy the assets in place now, but you can also do that after completing the setup phase. Tap *Next* to proceed.

    ![Cover](img/config_android_director_step_7.jpg)

8. The channel configuration is now created and the setup phase has been completed. Tap *OK* to return to the *Home* screen.

    ![Cover](img/config_android_director_step_8.jpg)

    !!! note
        Channel configurations are stored to your device's permanent memory (you can close the app and power off the device). They will also survive updating the app to the latest version. However, if you reinstall the app for example to change between the store version and the beta version, the channel configurations will be lost and you need to re-create them. Notice that you will not get the same channel numbers, as they are given randomly.

9. Your new channel configuration now appears on the *Home* screen. If you create many channel configurations, swipe them to left or right to find the one you wish to use.

    ![Cover](img/config_android_director_step_9.jpg)

10. If you need to edit an existing channel configuration, long tapping a channel configuration will bring its editing controls in view. Tap the cog wheel to return to the *Setup* screen where you can edit the configuration. Tap the cross to delete the channel configuration. Tap anywhere else to hide the editing controls.

    ![Cover](img/config_android_director_step_10.jpg)

11. If you long tap the channel configuration and then tap the cross button, a confirmation dialog is shown. Select *OK* to permanently delete the channel configuration.

    ![Cover](img/config_android_director_step_11.jpg)

    !!! warning
        This action cannot be undone. Once you confirm removing a channel configuration, you have to re-create it from scratch to get it back. Notice that you will not get the same channel number, as they are given randomly.

#### Oculus

Currently, the director mode is not supported on VR-only devices such as GearVR and Oculus Go. You cannot use these devices for controlling a presentation. However, you can configure them to the audience role and view a presentation. This is explained [later in this chapter](configuration.md#oculus_1).

### Audience Role

#### iOS & Android

In a device group, all but one device must be configured to the audience role. These devices are often iOS or Android phones and tablets. The configuration is very similar on both platforms.

Follow the steps below to configure your device to the audience role:

1. Start the LiveSYNC app. The *Home* screen appears. Initially, channel configurations do not exist. To create a new channel configuration, tap the big (+) button.

    ![Cover](img/config_android_audience_step_1.jpg)

2. The *Setup* screen appears. First, tap the *Audience* button to select the audience role.

    ![Cover](img/config_android_audience_step_2.jpg)

3. Your selection is marked by underlining it, as in the image below. The selected role also appears in the setup progress menu on the left. If you are using a phone, a new page *View mode* appears at the end of the progress menu (it is related to VR mode). Tap *Next* to proceed.

    ![Cover](img/config_android_audience_step_3.jpg)

    !!! note
        Current setup page is underlined in the setup progress menu on the left. You can navigate through the setup pages by tapping the page titles in the progress menu, by swiping the page towards left or right, or by tapping the *Next* button on the bottom right corner. On Android, you can also use the device's *Back* button to return to previous page.
        
        Your input is validated on each page. You cannot proceed to the next page before your input is accepted. If you return to the first page and change the role, your input to the other pages is cleared.
        
        If you want to cancel channel configuration, tap the *Home* button on the top left corner and answer *OK* to the confirmation dialog that appears.

4. Other users can identify you by your LiveSYNC name. This can be for example your own name, a name that you have given to your device, or your device's model name. The name cannot be left empty. Its maximum length is 32 characters. Tap the text field to type a name. Tap *Next* to proceed.

    ![Cover](img/config_android_audience_step_4.jpg)

5. Communication between the control device and the viewing devices is based on creating a wireless connection. The currently available connection types are listed. Choose a connection type that you wish to use. Notice that **the director device and the audience devices must use the same connection type**. Tap *Next* to proceed.

    ![Cover](img/config_android_audience_step_5.jpg)

    !!! note
        A connection type that is supported by your device and your LiveSYNC software version may still be unavailable. If so, it is marked as *Not available* in the list. Tap the info button (i) next to it to learn why it is not available. As an example, you may need to enable Wifi or Bluetooth feature from the device's settings. Use pull-to-refresh gesture to update the list after fixing the issue.

6. Devices that are using the same connection type and the same LiveSYNC channel can exchange messages. Devices on a different channel will not see them. Tap the text field to type a channel number. Use the same channel number that you configured to your control device. The channel numbers are in the range 1000-9999. Tap *Next* to proceed.

    ![Cover](img/config_android_audience_step_6.jpg)

7. If you are configuring a phone, select the view mode. If you plan to use Google Cardboard or similar passive VR headset, select *VR*. Else, select *Normal*. Tap *Next* to proceed.

    ![Cover](img/config_android_audience_step_7.jpg)

    !!! tip
        You can change the view mode also during a presentation by long tapping the screen.

    !!! note
        This page does not appear on tablets. Tablets are physically too large to be used in VR mode.

8. Android only: a dialog appears to ask your permission to access the files on your device. Without a permission the LiveSYNC app cannot create the directory where your assets will go. Also, it cannot read from this directory even if you create it manually. Tap *Allow* to give file access permission.

    ![Cover](img/config_android_audience_step_8.jpg)

9. The channel configuration is almost complete. This setup page reminds you that the presentation's assets must be copied to the device. This task will be covered in detail in the next chapter [Managing assets](asset_management.md). You can copy the assets in place now, but you can also do that after completing the setup phase. Tap *Next* to proceed.

    ![Cover](img/config_android_audience_step_9.jpg)

10. The channel configuration is now created and the setup phase has been completed. Tap *OK* to return to the *Home* screen.

    ![Cover](img/config_android_audience_step_10.jpg)

    !!! note
        Channel configurations are stored to your device's permanent memory (you can close the app and power off the device). They will also survive updating the app to the latest version. However, if you reinstall the app for example to change between the store version and the beta version, the channel configurations will be lost and you need to re-create them.

11. Your new channel configuration now appears on the *Home* screen. If you create many channel configurations, swipe them to left or right to find the one you wish to use.

    ![Cover](img/config_android_audience_step_11.jpg)

12. If you need to edit an existing channel configuration, long tapping a channel configuration will bring its editing controls in view. Tap the cog wheel to return to the *Setup* screen where you can edit the configuration. Tap the cross to delete the channel configuration. Tap anywhere else to hide the editing controls.

    ![Cover](img/config_android_audience_step_12.jpg)

13. If you long tap the channel configuration and then tap the cross button, a confirmation dialog is shown. Select *OK* to permanently delete the channel configuration.

    ![Cover](img/config_android_audience_step_13.jpg)

    !!! warning
        This action cannot be undone. Once you confirm removing a channel configuration, you have to re-create it from scratch to get it back.

#### Oculus

TODO
