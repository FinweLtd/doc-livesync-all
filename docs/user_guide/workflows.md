![Enterprise feature](../img/enterprise_feature.png)

## Camera Path Normalization

### How to use path normalization? 

1.    Use a cam path that's not already normalized to same real-world coordinates.
2.    In editor open new or saved the project.
3.    You need to place three calibration point type hotspots and set real-world positions in properties. They also need to have calculated world positions by using auto tracking.
4.    "Normalize" button appears, click that and confirm.
5.    After normalization in 3D map make sure that the path looks good and calibration point spheres are aligned with the three cross-shaped objects that are real-world reference positions.
6.    Saving the project saves the hotspots and creates a copy of this normalized path in the same folder with "_normalized" postfix e.g. someCamPath.mp4_normalized.txt
7.    Optionally you can now delete calibration points if you wish.
8.    After normalization, you can denormalize using the button. For now, all it does it delete the normalized cam path and forces to reload project with nonnormalized cam path. That means if your hotspots are placed in normalized cam path then they won't appear in the correct positions in nonnormalized cam path. In normalization, all hotspot positions are converted to new normalized coordinate but same for denormalization has not yet been implemented.


**Watch a tutorial video on camera path normalization**

<iframe src="https://player.vimeo.com/video/283704649" width="640" height="481" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

*Video not working? Click [here](https://vimeo.com/283704649/bba2c9e5d4) to open it in Vimeo.*

!!! Note

    - Original cam path is not modified by the normalization.
    - If you didn't save your project then you need to normalize again when you load your project.
    - You can freely move hotspots in 3D space by changing position values in hotspot properties.
    - For more accurate path normalization it's better to have calibration points as far apart as possible from each other.