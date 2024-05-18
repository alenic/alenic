```bash
$ python -c '''
import numpy as np
import cv2

img = cv2.putText(np.zeros((8,78)), "Hello World !", (0,6), 3, 0.25, 255)
print(*["".join([[" ","#"][int(img[i,j]>0)]for j in range(78)])for i in range(8)], sep="\n")
'''
```
```bash                                                                 
 ## ###    ## ##          ######         ##   ##      #                       
 ##  #      #  #          #####           #    #      #                       
 ##### #### #  # ####      #### #### #### # ####      #                       
 ##  # #### #  # #  ##     #### #  ## #   # #  #      #                       
 ##  # #  # #  # ## ##     # #  ## ## #   # ## #                              
 ## ### ######### ###      # #   ### ### ### ####     #  
```
Hi 👋 I am Alessandro!

**Aritifcial Intelligence** is my passion and job. My main specialization is in **Computer Vision**, but I am working in many other areas as well, like NLP and Multimodal Learning.

I appreciate feedback and contributions!

If you want to contact me: [Linkedin Profile](https://linkedin.com/in/alessandro-nicolosi/)
