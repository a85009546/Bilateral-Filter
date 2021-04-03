# Bilateral-Filter

* A edge preserving denoising filter


spatial filter -> denoising

range filter -> edge preserving

![image](https://github.com/a85009546/Bilateral-Filter/blob/main/bilateral_work.png)

$$Ip' = (sum_{Gs(i, j) * Gr(i, j) * Ip}) / (sum_{Gs(i, j) * Gr(i, j)})$$

$Gs(i, j) = (1 / 2*pi*sigma_s) * exp_{- (i^{2} + j^{2}) / (2*sigma_s^{2})}$

two tips to speed up the algorithm : 
1. building the look-up table for 
