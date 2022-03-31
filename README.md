# Robust-MPC-approaches-for-monotone-systems
Repository including all calculations for the case study of the eponymous paper.

## Abstract
This paper exploits the efficient computation of
reachable sets for monotone systems to formulate model predic-
tive control approaches with guaranteed constraint satisfaction
and recursive feasibility in the presence of uncertainty. To
include all realizations of uncertain parameters, the reachable
sets are approximated as hyperrectangles in the problem
formulation. The presented approach is extended to include
recourse, i.e., the knowledge about the presence of further
measurement information in the prediction horizon. By dividing
the reachable sets, multiple regions are obtained, for which the
future inputs can be chosen separately. The applicability of the
proposed approaches are shown by the means of a temperature
control example.

## About this repository

Thank you for looking into the supplementary code!
All the calculations presented in this paper were done in Python and can be reevaluated in the Jupyter Notebook.
The main toolboxes used for this are:

- numpy
- matplotlib
- CasADi

As well as our own toolbox [do-mpc](www.do-mpc.com).

If some questions arise, please feel free, to contact [me](moritz.heinlen@tu-dortmund.de)!
