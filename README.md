<table>
<tr>
<th> Code </th>
<th> Output </th>
</tr>
<tr>
<td>

```python
import cv2
img = cv2.resize(cv2.imread("alenic.jpg", 0), (34,24))
h,w = img.shape
Q = 9
gray_chr = " .-:!*+x#@"
img = 255-((img*(Q/255)).round()*(255/Q))
img = (img*Q/255).astype(int)
print(*["".join([gray_chr[int(img[i,j])]for j in range(w)])for i in range(h)], sep="\n")
```

</td>
<td>

<img src="out.png" alt="drawing" height="180"/>

</td>
</tr>
</table>



Hi 👋 I am Alessandro!
🧠 **Artificial Intelligence** is both my passion and profession. While my primary specialization is in **Computer Vision**, I am also actively working in other areas such as **Natural Language Processing** and **Multimodal Learning**.

In my free time, I like experimenting with **Reinforcement Learning**.

❗️I welcome and appreciate any feedback and contributions.

🌐 Contact: [Linkedin - Alessandro Nicolosi](https://linkedin.com/in/alessandro-nicolosi/)
