+++
title = "Mux and dmuxes"
date = 2026-10-29T00:00:00+05:30
type = "notes"
url = "/notes/optical/mux-and-dmuxes/"
+++

so these are basically the select and deselect type of nodes on the basis of these gates, one useful case could be like 
![Pasted image 20260112132145.png](/notes/optical/assets/Pasted%20image%2020260112132145.png)

over a communication line, you can interleave multiple digital signals together by using something called the *oscillator* and a dmux can just seperate these things out, digitally i get it
- but what about the light based, you can have multiple signals interleaved at different wavelengths, and since you might need to channel them, but maybe not? because your wire supports *multiple data*
- these sorts of operations could be asynchronous, how. would that work for photonic based stuff
	- the multiplexing we are doing in the digital / electronic system is based on time, it is called time based multiplexing which is useful to use a *clock* to send multiple data bytes interleaved over the same network
	- so in photonics, we dont really need that because the different wavelength of light is enough to create a new channel
		- red carries some other data
		- blue carries some data
		- dmuxing is not done by elaborate electric circuits, you can just put a grating / blocker of other types of wavelength of lights. i do wonder what would be the mechanism of operating those gratings...
			- prolly something electromagnetic.