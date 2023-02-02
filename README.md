# effseq

This project explores algebraic effects in the Curry-Howard interpretation of certain sequents as programming language feature.\
In the calculus here, the sequents emerge either from a natural deduction (ND) proof calculus (left introduction and elimination) together with an additional right elimination or a ND refutation calculus (right introduction and elimination) together with an additional left elimination.
The cut in the sequents separates an ND elimination on the left/right from an elimination on the right/left.
That is, the cut is a delimiter of a proof/refutation context.
This opens the door for an an algebraic effect in an inhabitant of a sequent.

So far, the project consists of a paper sketch containing a formulation of the above idea and some concrete example programs to play with which are temporarily gathered in the introduction section.
Moreover, the calculus seems to be type- and effect-safe and even consistent (except for the inconsistencies which are introduced axiomatically to be able to write closed programs, of course).\
Alas, a motivation for the system is still lacking, preventing any further work.

## Installation

Just call `make bib` at the top-level of the repo.

## Contributing

Contributions are welcome!
We are glad about any kind of help.
Just use Github Issues and pull requests as you would for any other project.

### Style

If you contribute text, please follow [Dreyer's notes on writing papers](https://people.mpi-sws.org/~dreyer/talks/talk-plmw16.pdf).

## TODO

Before doing anything else one has to find a real argument for the usefulness of the system.
So finding such an argument is the only thing to do at the moment.\
In that regard, note that the obvious application domains are
- proof assistants due to the presumably consistent logic it is built on.
- intermediate languages due to [prior promising results with sequent calculi in compiler pipelines](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/04/sequent-calculus-icfp16.pdf).
- object-oriented programming due to [the nature of codata](https://blog.shtsoft.eu/2022/11/25/mot-oop.html).
