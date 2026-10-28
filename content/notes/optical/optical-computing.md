+++
title = "Optical computing"
date = 2026-10-29T00:00:00+05:30
publishDate = 2026-10-29T00:00:00+05:30
written_date = 2026-03-28
type = "notes"
url = "/notes/optical/optical-computing/"
+++

the goal is to get a rough idea of the map, and put pressure on one aspect of it, and see what you can contribute

the goal post has changed, the goal is to learn, given optical computers, do exist and can exist, how can you (*goal: exploit high bandwidth, extreme parallelisation*) assuming somewhat normal memory and normal logic gates exists
- memory you can't honestly comment much
- the machines are non-von neumann based
- what are the fundamentals?
	- compsci large ideas hold
		- you'll still have an architecture
			- you'd still require some sort of isa
					- and post isa it is not that simple as well, like there exists multiple things within architecture (isa, assembly language, opcodes and instruction) and down that level the microarch is where the particular implementations differ knowing both is important
				- [[comp arch and microarch]]
		- you'll still have a OS, Compiler translating things down
		- 
	- theory of computation
		- clocks are still always there
		- machine is still going to change state in one way or the other
	- architecture principles? boolean algebra + ideas that lead to development of von-neumann type architecture?

- optical gates are one thing, what are the building blocks and architecture of such devices
	- useful for knowing the core foundation
		- what are the building blocks of optical logic gates
		- are the normal and nand gates specify our needs?
	- knowing these, lets you directly take cs comp arch theory and  directly paste it into photon based chips
- chatgpt says that the action is at ai + photonics rather than classical computing
	- in terms of goal setting chatgpt suggests me to build
		- [[fourier optical processor]] (concept -> optical convolution)
			- we are doing a fourier optical processor then
			- this is where i start i guess, using light source for doing actual stuff.
		- fiber optic inferometer
		- 1-bit neural network element
		- goal 1 acc to me is to spend a week or two just getting to read about it and build questions around the subject that you can send to michael and 2-3 other researchers in the field
		- see these things are cool and useful application of the real irl stuff but the name of game is *non-linear optics* this the the shtuff behind making of logic gates
	- these projects also require physical stuff to work with so that you understand somewhat the physics of it, but obviously i am interested in the computational and physical both aspects of it
- some clauding, it suggest me to NOT delve into the physics, just understand upar upar se what stuff is, and my maximum energy should go into RISCV and architecture papers
- starting from computational optics seems like a better bet. 
	- so see you want to work on the actual thing, so learn what lets you work first, rather than just theory
	- akhetronics is
		- designing the chips
		- doing the work required to run stuff like 'doom' on their hardware
		- they are building an 'ISA' that works on the optical chip
		- something something riscV for this shite
			- i get it now, the level i wish to operate is very computer-sciency
			- they have the hardware, I learn enough of the hardware to appreciate is somewhat
			- after spending some time on this, there is obviously a very deep-physics layer that i dont want to get into rn, because that is not my goal rn, some recalliberation suggest that
				- i want to work with them, so in terms of exciting is how would that ISA work what would they do to work with that layer. if we have the hardware, and more importantly i want to do something around that
			- i am interested in the problem of architecture or code that i write that makes it work on the chip
			- *the ideal project* would include me coding up something using a computational optics library, (since i dont have those physical computers right now) and focus on using now that i am on the hardware what do i do with it.
			- i think I am right on what these folks are doing
		- gippity says it right - *Build a RISC-for-light toy architecture and run code on it in simulation*
			- the only next logical question is what is RISCV XD
			- so so we have HDL right which is an assembly variant like thingy, now you have to essentially do that, using your photonics arch
			- oh god oh god where do i start this is so cool
---
### wiki

basically using incoherent sources of light for the processing, storage and computation of data
why use them at all? they offer higher bandwidth than the electrons?

*why do they offer higher bandwidth than electrons?*
- like it might due to the drift velocity and stuff in electric wires
	- wiki talks about exactly this being the reason for optical computers to be very fast, as they can have insanely high frequencies
- but i have no intuition on how light behaves and works, in physical media
	- like learning about light in that context, comparing formulae's and data

also the optical folks still want to play bitwise only
- key issue with this approach
	- this is based on the short-term, because a lot of energy in "optoelectronic" device to convert electronic energy into photonic
		- *so could their be a totally a photonic transfer of data & energy?*
			- based on theory it is possible
			- did akhetronics or other lightmatter folks have done that?
		- *how is energy efficiency right now?*
			- in pure electrical basis using our bits and bytes.
	- these transitions are call OEO (optical electronic optical) **conversion** of energy
	- there is something called *optical correlator* that operates on *fast fourier transform* which seems to be the most fundamental calculation or method in optical computing
- a redditor talks about how there are some application where this nature of waves is fundamentally superior to those of electrons for eg, summation of something is much better using all optical fibers pouring their intensities into one?
	- well cant you do that with electrons, what's the difference?
		- i mean the keyword i heard was *ai inference* 
			- some gipptying told me that inference is essentially the running of an ai model which takes most of the energy now a days, how does the optical computer rank here?
			- optically the process of inference which is a summation of different probabilities i guess would be much better on a optical chip because *you dont need energy, and can use waveguides i.e using literal structure to do computation*
				- this is a claim i need to learn about how true it is
				- if it is true learning the physics & maths behind this is obviously natural.
	- in the end redditor says how using electronic computers are not a physical limitation\
		- we know that akhetronic played doom on a computer like that
			- so they have already done advanced work in the domain
- basic key idea is that we need a transistor equivalent built using photon principles, they call it the *optical switch*, they use something called crystal optics, using non-linear refractive indices which is interesting because maybe you can control refractive indices
- now that we know the fourier properties of lenses, we are limited by the speed of converting electrical to optical signals and so forth
	- so the question is *what architecture has the akhetonics people* suggested are there 
	- are there OEO conversions or not?
- there is a lot of other parts of the field as well
- the best way to start now is actually build something, either computational or physical
---
gipitty suggests to learn minimum electrodynamics & stuff

### See also
[[problems with current computers]]
quantum effects
[[optical image processing]]
[[non-linear optics]]
[[optical architecture]]
neural networks
akhetonics