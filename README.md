## bonsai_tracking_playSoundUponMovement_2regions
</br>

## bonsai_tracking_playSoundUponMovement_2regions_1active

bonsai_tracking_playSoundUponMovement_2regions_1active is like bonsai_tracking_playSoundUponMovement_2regions but:
- it plays sound2 in ROI2 whenever the mouse is in ROI2 regardless of its movement speed; no sound is played when mouse is in ROI1.
- It uses centroid velocity instead of frame difference between consecutive frames

### Parameters

![image](https://github.com/lachioma/bonsai_tracking_playSoundUponMovement_2regions/assets/29898879/714f58c2-652b-4f35-9fb6-93b1d420b90f)

**ThreshGrayValue**: Default is 56. Threshold to binarize image and then detect mouse, it should be set just higher the brightness value than the mouse body.

**ThreshVel**: Default is 5. Velocity threshold to trigger ToggleMovement.

</br>
</br>
</br>

![image](https://github.com/lachioma/bonsai_tracking_playSoundUponMovement_2regions/assets/29898879/38912537-f2d6-43ac-a52e-899457d44036)

**FindContours – MaxArea and MinArea**:

 Minimum and maximum number of pixels for object detection.
 Set it to the expected size of the mouse.
 You can try to set MinArea quite high to exclude artifacts of the tail when the mouse is in between ROIs.

N.B. There is one distinct FindContours for each ROI!


