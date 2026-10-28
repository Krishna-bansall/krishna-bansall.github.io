+++
title = "Akehtonics arch paper"
date = 2026-10-29T00:00:00+05:30
publishDate = 2026-10-29T00:00:00+05:30
written_date = 2026-01-03
type = "notes"
url = "/notes/optical/akehtonics-arch-paper/"
+++

- so basically they are arguing first of all that non von neumann architecture doesnt mean our code wont run on it
	- you can always do the computation exactly in the same way then in diff architecture
- so sometimes instructions are measured on the basis of cycles they take per instruction? cycle being i computation by processor
	- but they are arguing in a simple architecture, instead of caring for micro-optimising instructions you can use a lot of instructions parallely aka *SIMD*
		- although they recognise that simd is only limited to the clock speed here, which again is in the terrahertz (thus making do with a few thousand instructions) but i would also guess that the speed limits of light makes it easier to not-requiring compressing everything down to be very close!
	- you may think now you have gone completely into comp-arch vicinity & wasted the time doing physics but that is just sunk-cost fallacy.
- so at highers scales parallelisation might have diminishing results abut they know since a lot of ai work is vector multiplication using these chips just might be it because, [[fourier optics]] secondary property of lenses, matrix multiplication linear operations VERY FAST.
- The author makes a point, that you can basically do everything you want with even a 100 logic gate architecture & parallelisation with most of the extra logic gates being added for the sole purpose of optimisation & speed.
- they are using 2 bit cpus, but they are mostly referring to how many bits a cpu can operate on and not just the address space for the cpu because that would result to only 4 memory locations, thus I need to look into this part (read theory)
	- and for higher number representations such as 32 bit numbers using your 8 bit numbers, you can combine 4 x (8-bit) integers to make a 32 bit numbers, thus storing 32 2-bit integers you can represent a 64 bit number (but doesnt that seem to be a awfully lot of integers?) but one does think how terrahertz of speed affects that.
	- they admit it would require more steps but they are asking us to keep an open mind with the fact that things could be done and the only reason we are seeking these computers are there unparalleled ability to do other computations (at the speeds of light mind-you!)*
- they consider 4-bit & 8-bit architectures to be the sweet spot (as it require **o(n^2)** no of logic gates to do simple arithmetic operations via LOGIC GATES) 
	- they are admitting that this stuff leads to loss in precision but! makes the our stuff faster
	- they are looking at 16 bits, as a fair trade to to do their calculations & shite
	- they are suggesting doing most stuff with 16 bits as most values dont exceed 65K, & they are okay taking some performance hit. & using simd for parallelisation of ai tasks

- reversible computing?
- non-linearities allow doing / creation of almost instantaneous *all-optical switching devices*
	- this enables *time of flight computation*
- write once read many (WORM) memory 
	- so one of the properties of these memories is that they are easier to write to first, and read as many times, but the second rewrite could take upwards of 100x the initial operation.
	- they are suggesting that the vast majority of computing operations are LOAD (which this memory is good at) and the main benefit of transport speed being around 1ns (at max tho) as compared to the electrical 80-90ns rougly 100x imoprovement
	- people critique this approach being experimental but they have mentioned some research that shows that this type of memory can be used as ram (*this does show a lot of potential for manufacturing business on this side*)
	- they have identified problems with memory 
		- it also seems to be somewhat of a point contention they have
		- this would require a new-computing paradigm as the natural push would be towards compiler-based & software based solution initially
		- turing awardees have cared for using this sort of system, it supports functional programming, not sure how but it does
			- the principles of functional programming, requires to use immutable data, and akhetonics folks seems to be suggesting that it is not always the case for compilers thus they have to develop this as well, *they require instruction set level immutability*
			- this is also aligned with reversible computing? (*crazy stuff*)
			- there are 2 new paradigms as of now, functional programming is there and reversible computing also exists, it seems like a FUTURE thing tho
---
the world aint binany
- sure you are not limited to digital processing, you can do analog stuff as well, use that nature well




- *you should have an idea about what a neuromorphic circuit is so you know what is going on in the chip*
- *I need to verify the claim about how can a 100 optical gate computer work using SIMD and shit as compared to a normal computer*
	- *If the claim seems good enough you can definitely run simulations on that*
	- *know what SIMD does & how it works*
- *read theory on data buses, bit width and alike on cs:app*
- *i am skeptical about how good are 4-bit & 8-bit processors for computre*
	- *read the graphs & try to understand them*
- *what are all optical switching devices*
	- *what do they do?*
	- *what the concept of switching*
	- *what is time of flight computation*
	- *what is latency in switching?*
		- *what is fucking adiabetic & reversible logic in computing!*
			- *what is Landauer’s principle?*
				- *learn about it & look at it from their perspective*
				- *look if its a shiny new thing or something impactful*
- *learn about miller's criteria*
- *learn how RWORM Memory works and get to know some of its limitation grok the paper referenced as [74]*
	- *what are Copy on Write [COW] mechanism?*

---
[[computer architecture]]

---
[[photonics project]]