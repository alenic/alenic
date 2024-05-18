```bash
$ python -c '''
import numpy, cv2, sklearn
import sklearn.preprocessing
img = cv2.imread("alenic.jpeg", 0)
img = cv2.resize(img, (32,16))
h,w=img.shape
img = (numpy.round(img*(8/255))*(255/8)).astype(int)
img = sklearn.preprocessing.LabelEncoder().fit_transform(img.flatten()).reshape(h,w)
print(*["".join([" .:-+*x@"[int(img[i,j])]for j in range(w)])for i in range(h)], sep="\n")
'''
```
```                                                                 
::::::::::::::::::::::::::::::::
::::::::::::*-:---  ::::::::::::
:::::::::: -:::::::::.::::::::::
::::::::: ....:-::.:x: :::::::::
::::::::...xxxxxxxxxxx. ::::::::
::::::::...+xxxxxxxxxx+.::::::::
::::::::..+xxxxxxx+++-+.::::::::
::::::::++::..:+x+:..::+.:::::::
::::::::++xxxx@xxx*xxxx*.:::::::
:::::::-+++xxx@xxxxxxxx+::::::::
::::::::: :+:++:::+++-: ::::::::
:::::::::: :++:::::+++ :::::::::
::::::::::: +xx::+xx+ ::::::::::
:::::::: -:+:.:+x+.::++.-   ::::
::::- -....+++:::::+++......--- 
-............++++++-............
```
Hi 👋 I am Alessandro!

**Aritifcial Intelligence** is my passion and job. My main specialization is in **Computer Vision**, but I am working in many other areas as well, like NLP and Multimodal Learning.

I appreciate feedback and contributions!

If you want to contact me: [Linkedin Profile](https://linkedin.com/in/alessandro-nicolosi/)
