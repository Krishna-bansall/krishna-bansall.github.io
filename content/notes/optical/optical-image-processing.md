+++
title = "Optical image processing"
date = 2026-10-29T00:00:00+05:30
publishDate = 2026-10-29T00:00:00+05:30
written_date = 2026-10-07
type = "notes"
url = "/notes/optical/optical-image-processing/"
+++

optical images and signal processing, why learn about them, what are they?
- lenses have a fourier transform property (which is not trivial)
	- there is something called [[fourier optics]]
i think they are trying to say

- see frequency has a lot of relation with the images, low frequency within images usually depicts more colorful and high brightness ares
- and the higher frequencies show darker and sharper stuff.

let's imagine an image as a 2D function 
what are spatial & temporal frequencies?

----
### Representing images as frequencies

- **Representing 1D functions**
	- fourier tells as that any curve can be expressed as a sum of sine curves of different frequencies 
	- *nyquist rate* - no of samples required to form a given curve i.e no of samples required to produce the highest frequency curve
![Pasted image 20251231170933.png](/notes/optical/assets/Pasted%20image%2020251231170933.png)

- **Representing 2D functions aka images**
	- you use frequency curves which are basically black and white gradient lines, multiplying or doing operations with these lines lead you to understand what is going on with images
	- ![Pasted image 20251231172332.png](/notes/optical/assets/Pasted%20image%2020251231172332.png) 
	*Sum of 2 simple curves.*

Now the question arises that how does our friendly mathematical fourier transform helps with images, we know that 
- in maths 
	- the transform leads to the 1d plot of all frequencies with noise that are present in a given function
- ![Pasted image 20251231181358.png](/notes/optical/assets/Pasted%20image%2020251231181358.png)
now i have gotten a basic intuition for low pass & high pass filtering & why are images represented the way they are
- Now the question arises, what do lenses have to do with it & how does it have fourier properties? 
- how are we getting a free transform

---
![Pasted image 20261007134011.png](/notes/optical/assets/Pasted%20image%2020261007134011.png)

we can also sort of understand the transform as a part of zhi - 1 and zhi - 2 : that is x,y components of the frequency domaink