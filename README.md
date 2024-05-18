```bash
$ python -c '''
import numpy, cv2, sklearn
import sklearn.preprocessing
img = cv2.resize(cv2.imread("alenic.jpeg", 0), (34,16))
h,w = img.shape
img = 255-(numpy.round(img*(5/255))*(255/5)).astype(int)
img = sklearn.preprocessing.LabelEncoder().fit_transform(img.flatten()).reshape(h,w)
print(*["".join([" .:x#"[int(img[i,j])]for j in range(w)])for i in range(h)], sep="\n")
'''
```
```                                                                 
::::::::::::::::::::::::::::::::::
::::::::::::#.:x:::.#:::::::::::::
::::::::::::xxxxxxxxxxx#::::::::::
::::::::::#xxxxx:xxxx xxx:::::::::
:::::::::#x             #:::::::::
:::::::::#x.            x#::::::::
:::::::::#x         ..x.x#::::::::
::::::::#..xx#xx. .xx#xx..#:::::::
::::::::#..        .    ..#:::::::
::::::::#..             .#::::::::
::::::::::#.xx.:xxx:..x.#:::::::::
:::::::::::x...::x::....x:::::::::
:::::::::::#x.  xx.  .x#::::::::::
::::::::##:..xx:. .:xx..xx:###::::
:::::#xxxxx....xxxxx:...xxxxxx:::#
:xxxxxxxxxxxxx......:xxxxxxxxxxxxx
```
Hi 👋 I am Alessandro!
🧠 **Artificial Intelligence** is both my passion and profession. While my primary specialization is in **Computer Vision**, I am also actively working in other areas such as **Natural Language Processing** and **Multimodal Learning**.

In my free time, I like experimenting with **Reinforcement Learning**.

❗️I welcome and appreciate any feedback and contributions.

🌐 Contact: [Linkedin - Alessandro Nicolosi](https://linkedin.com/in/alessandro-nicolosi/)
