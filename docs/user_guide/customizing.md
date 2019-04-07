# Customizing

[comment]: <> (Settings file, custom branding(how to add your own background/waiting room) )

## Customizing LiveSYNC 

For LiveSYNC there is settings file that can be used to customize LiveSYNC's user interface, channel and, tabs. The settings file can be edited and saved under LiveSYNC folder. The settings file is a mix of boolean (true/false), numeric, and string values. 

If you wish to open a given channel number every time you launch the application you can define the value as follows:  

    ; automatically opens given channel on startup, true/false
    default_channel_on_startup=true
    ; channel number between 1000-9999
    default_channel=1000
    
If you have own contents and wish to hide demo contents from Player view, it is possible to do so by using the following attributes:

    ; demo assets that come with the app
    [demo]
    ; minimize "Demo Content" section in the content tab, true/false
    demo_content_minimize=false
    ; completely hide "Demo Content" section, true/false
    demo_content_hide=false
    ; minimize "Demo Set" section in the tags tab, true/false
    demo_tags_minimize=false
    ; completely hide "Demo Set" section, true/false
    demo_tags_hide=false
    
LiveSYNC's player tab is a mix of multiple tabs. One might need all tabs and one might want to hide the tabs. 

![Workspace](img/workspace_director_3.png)

It is possible to hide or minimize the tabs by changing the boolean value to true. 

    [tabs]
    ; minimize "Devices" tab on start, true/false
    devices_tab_minimize=false
    ; completely hide "Devices" tab, true/false
    devices_tab_hide=false
    ; minimize "Tags" tab on start, true/false
    tags_tab_minimize=false
    ; completely hide "Tags" tab, true/false
    tags_tab_hide=false
    ; minimize "Content" tab on start, true/false
    content_tab_minimize=false
    ; completely hide "Content" tab. In editor this also hides tags tab, true/false
    content_tab_hide=false
    ; completely hide "Properties" tab from editor, true/false
    properties_tab_hide=false
 
The settings file will give you the chance to tailor LiveSYNC the way it suits your content, audience and presentation nature. Note that a line that starts with semicolon **(;)** is a comment. A comment is added for the purpose of making the settings file easier to understand and it is ignored by LiveSYNC. Click [here to download settings.ini](..//downloads/downloads.md#settingsini).


## Custom branding 

 ![Enterprise feature](../img/enterprise_feature.png)
 
 Custom branding is one extra benefit you can get by using the enterprise version of LiveSYNC. Using custom branding you have the possibility to change the waiting room's lounge background also known as [a lobby](..//user_guide/workspace.md#lobby) on the audience's view, put own logo in the screen and use own logo on exported reports. 
 
 In order to customize LiveSYNC, you need three image files: **lounge_background.jpg** a 360-degree waiting room background, **lounge_logo.png** logo that can be seen in the screen, and **report_logo.png** logo for the report. The three files need to be in a folder by the name *CustomBranding*. 
 
  ![Custom branding](../img/customBranding.png)
  
  ![Custom branding](../img/customBranding1.png)
 
 Copy the *CustomBranding* folder to both the director and **all audience devices** LiveSYNC folder. To get a better idea where to copy the folder, take a look at our tutorial on [Where Should My Files Go?](..//user_guide/asset_management.md#where-should-my-files-go)
 
!!! note
    The changed lobby background is seen in all the audience devices, not on the director iPad.  
    
 ![Enterprise feature](../img/enterpriseFooter.png)  