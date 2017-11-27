# MIPS

A MIPS hardware design for the Computer Design Discipline (6th semester) Computer Engineering @ [Insper](https://www.insper.edu.br/en/).

## The Processor

Implemented pipeline version of the [MIPS processor](https://en.wikipedia.org/wiki/MIPS_architecture).

The concept was to develop a MIPS architecture processor in VHDL, that would run on a Altera FPGA board.

With the goal of learning computer design by doing, we implemented a instruction-set of 9 instructions, that run in a pipeline.

<!-- ### Diagram -->

<!-- ![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "MIPS pipeline Diagram") -->

<!-- in black: the Dataflow -->
<!-- in red: the Control unit -->

### Implementation

*Top Level Entity:* [MIPS](./MIPS.vhd)
Handles the interaction between the [Dataflow](./FluxoDeDados.vhd) and [ControlUnit](./UnidadeDeControle.vhd)

### Limitations

## implemented instruction-set

Our MIPS instruction set counts with the following instructions:

#### R-Type
- ADD
- SUB
- AND
- OR
- SLT

#### I-Type
- LW
- SW

#### J-Type
- BEQ
- JUMP

## Next-Steps

- *Hazard prevention*
- Modular Code
- Refactor using 'generic'
