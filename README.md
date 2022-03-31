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

The Jupyter Notebook is structured as follows:

First the Model with 4 Rooms is introduced and the simulator is created.
Then the Uncertainties and the external influences are defined/loaded. 
Then a nominal MPC controller gets defined and used, which produces parts of the results from Figure 2 of the paper. 
The Open Loop Approach was not used in this case study, but can be evaluated to see, that it produces indeed infeasible results.
The Closed Loop Approach follows next, which produces parts of the results from Figure 2 of the paper by varying the uncertainty functions.
For the simplified closed Loop approach, the robust control invariant set is computed interlinked for the whole prediction horizon.
These sets are then used for the simplified approach, which also produces parts of the results from Figure 2 of the paper by varying the uncertainty functions.
To compare the scalability with the states, the computation of an RCIS for specific times was done.
First with 4 rooms, i.e. 12 states and 6 disturbances
Second with 9 rooms, i.e. 27 states and 11 disturbances
Thirdly with 16 rooms, i.e. 48 states and 18 disturbances.

Finally the Post-Processing for Figure 2 is presented.

If some questions arise, please feel free, to contact [me](moritz.heinlen@tu-dortmund.de)!
