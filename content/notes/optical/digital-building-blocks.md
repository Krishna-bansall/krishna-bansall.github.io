+++
title = "Digital building blocks"
date = 2026-10-29T00:00:00+05:30
publishDate = 2026-10-29T00:00:00+05:30
written_date = 2026-01-13
type = "notes"
url = "/notes/optical/digital-building-blocks/"
+++

Now we leave the abstraction level of logic gates and start building upwards abstraction for eg a decoder

- now i have some issues, you could have come up with anything, why decoders? why multiplexers? wtf
	- why and how are you so precise that these are the building blocks you want, what gave rise to this functionality? what were you thinking about
	- why karnaugh? how does it work?
	- in reality would i want to use MUX's and Decoders i dont know? why not some other building block, SOP form etc are there but i dont like why these specific forms


- sequential logic stuff where you are basically aware of the things that happened before, you not only get input to current blocks but also input to blocks before, this is useful for making the computer time aware

computers are deterministic, and not magical in that sense.
0's and 1's are a good computer encoding scheme, thus is being used to do operations, we may be able to do buncha operations from sround these, so yeah abstraction is a really important construct, we can ask sombody to take us somewhere and may assume that they already know where that place and how to take us, but our instruction leads to a good outcome that is transportation of us

a computer directs the processing of information & and also performs the actual processing of information
- information, data, insight has to be processed upon somehow with the use of procedures maybe
- and the actual processing are the procedures in of themselves perhaps the computation that is happening in of irself

### Storage Blocks
- we mostly looked at how combinational circuits can be built and used, and they are useful because they can make very functional arithmetic and logical blocks, and using the truth tables and sop forms, you can basically do any function possible using boolean algebra
- and looking at the basis of those gates, if we get a bit into electricity part of it, its not as simple as high or low voltage, there are aspects of cmos gates flipping positive or negative charges, and these are basically used in your inverters and such
- now in semiconductor physics we also have a conception of negative charge that is an electron and the hole, which acts like a positive charge carrier, remember: dopings and those diagrams as such [[transistors]]


---
[[mux and dmuxes]]
[[half adder]]