### Introduction

[XPP](http://www.math.pitt.edu/%7Ebard/xpp/xpp.html) is a software by Bard Ermentrout for the analysis of systems of ODEs. **PyXPP** is a Python wrapper around XPP that allows you to conveniently query information from the ODE file, run integrations, and compute nullclines. The main strength of PyXPP lies in its the usage of [PLY](https://github.com/dabeaz/ply), a Python Lex-Yacc implementation, to build a full-fledged XPP lexer, parser, and code generator. This provides easy customisability, and differentiates PyXPP from other XPP Python wrappers such as [Py_XPPCALL](https://github.com/iprokin/Py_XPPCALL) and [xppy](https://github.com/jsnowacki/xppy).


### Features
- Read paramters, initial conditions, auxiliary variables, state variables, RHS of ODEs, and functions.
- Run numerical integrations.
- Compute nullclines (unique to PyXPP)
- Modify parameters, nullcline options, initial conditions ...

### Dependencies
- Python 3
- [PLY](https://github.com/dabeaz/ply)
- [SciPy](https://www.scipy.org/)
- [XPP](http://www.math.pitt.edu/%7Ebard/xpp/xpp.html). The latest XPP Ubuntu binary provided as `xppaut`. You may need to change permissions to executable. Many distros also provide the binaries in their repos, e.g. Debian, Ubuntu, Arch (AUR).

### Tutorial
A demo and tutorial can be found [here](https://github.com/markolenik/PyXPP/blob/master/wiki/demo/demo.ipynb).

### TODO
- Convert functions to actual Python lambda expressions.
- Directional fields.
- Add some other commands. The following commands are not yet supported but could be easily implemented: `table, bdry, volt, markov, wiener, solv, special, set, derived parameters, numbers, int, block pseudo-arrays`

### How to Cite PyXPP

If referencing PyXPP in a paper, please use

`Olenik, M. PyXPP. 2018. Available at: https://github.com/markolenik/PyXPP.`

And as BibTeX:

```
@Misc{pyxpp,
  author       = {Mark Olenik},
  title        = {Py{XPP}},
  howpublished = {https://github.com/markolenik/PyXPP},
  year         = {2018--2020}
}
```
