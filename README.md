Line detection by color and zone of interest Simple algorithm of a single image before taking out to line dection of a streamed video. We will only can find perfect-white line with this algorithm, which is very limited in reality. However, it's keep easy to understand before moving to something more sophisticated.  
@author: nguyenrobot

Firstly, we read the image and find some caracterstics of loaded image
![Image Credit : Udacity](test.jpg)
Image Credit : Udacity

We will define RGB thresholds for color selection, we will only chosse pixels that are near to white.
![frame_color_selection](frame_color_selection.png)

![frame_line_over_color_dection](frame_line_over_color_dection.png)

We will define our zone of interest defined by a simple triangle to eliminate any un-welcomed detection.
![frame_zone_of_interest](frame_zone_of_interest.png)

In the end, we obtain a quite acceptable line detection result based on color slection and zone of interest :
![frame_line_dection](frame_line_dection.png)
