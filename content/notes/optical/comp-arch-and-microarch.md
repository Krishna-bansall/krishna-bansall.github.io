+++
title = "Comp arch and microarch"
date = 2026-10-29T00:00:00+05:30
publishDate = 2026-10-29T00:00:00+05:30
written_date = 2026-01-25
type = "notes"
url = "/notes/optical/comp-arch-and-microarch/"
+++

this is a small learning zone,  you see:
- there are multiple types of microarch that differs in the ways they implemented or the sort of pipeline
	- there could be different things like in mem processing, seperation of mem and comp
	- how is data flowed, are there any sort of parallelisation
- architecture is all about how code is compiled, what assembly is, and all the other stages of that post hardware
	- you should have idea of assembly
	- you should realise the isa, and how are things being represented for one single architecture, how you can understand performance concerns


- while learning, practical building is useful - using verilog and stuff
- running with ideas of how microarch is working or how different implementation goes is useful
- understanding von-neumann and post neumann other forms of arch
	- datapath
	- simd
	- gpu
	- learning these is useful as it is more like a training in how people went about diff architectures, so that you can go about with your different arch!
- other parts like clocks, digital building blocks and stuff are there, but be mostly quantitative about it atm because you are trying to reason from an abstraction level that here we have these building blocks how to work fwd from that
![Pasted image 20260125133810.png](/notes/optical/assets/Pasted%20image%2020260125133810.png)