# Image Enhancement
Remove noise from image\
![](https://github.com/ThomasArtemius/Image-Enhancement/blob/main/noisy_charlie_chaplin.png)
## Process
Imagine 7x7 noisy image. We will perform denoising with median filter. Before we do that, the image need to be padded. The padding value is based from the outer pixel value from original image, so it kind of like an extension. Then perform the median with the kernel. Let's say within the region we have value of

|----|----|----|
| 19 | 21 | 21 |
| 1  | 88 | 90 |
| 8  | 88 | 21 |

Then the middle value will be sought. Those numbers will be sorted like this: [1, 8, 19, 21, 21, 21, 88, 88, 90]\
The median number would be 21
![](https://github.com/ThomasArtemius/Image-Enhancement/blob/main/median_demo_numbers.gif)
## Result
![](https://github.com/ThomasArtemius/Image-Enhancement/blob/main/Result%20Denoise.png)
### Analysis
Bigger Kernel -> Image Blurier
