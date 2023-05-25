Trace the Basketball
=====================
In this activity, you will learn to trace the basketball trajectory.

<img src= "https://s3.amazonaws.com/media-p.slid.es/uploads/1525749/images/10493877/sa2.gif" width = "480" height = "320">

Follow the given steps to complete this activity:

1. Plot the basketball trajectory
* Open the main.py file.

* Create a function goalTrack() and pass img and bbox in it.
* 
  `def goalTrack(img, bbox):`
  
* Add the coordinates and dimension of the bbox.

  `x = int(bbox[0])`
  
  `y = int(bbox[1])`

  `w = int(bbox[2])`
  
  `h = int(bbox[3])`
  
* Get the CENTER Points of the Bounding Box.

  `c1 = x + int(w/2)`
  
  `c2 = y + int(h/2)`
  
* Append the center points to the xCords and yCords.

  `xCords.append(c1)`
  
  `yCords.append(c2)`


* Draw the circles for centre of ball in every frame.

  `for i in range(len(xCords)-1):`

      `cv2.circle(img,(xCords[i],yCords[i]),2,(0,0,255),5)`
  
* Call the goalTrack(image, bbox) function.

  `goalTrack(image, bbox)`
  
* Save and run the code to check the output.


