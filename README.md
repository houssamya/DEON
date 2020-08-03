# MC-DAU
## Model Checking Dominance Act Utilitarianism

This code includes functions to allow for the model checking of automata with specifications in dominance act utilitarian deontic logic.

Finite weighted automata are defined as graphs of states and transition relations, given weights as edge properties, and prescribed actions via a dictionary of action names and edges. Automata can be model checked for obligations by defining an Obligation object that takes a LTL formula written in the nuXmv language to be converted into a CTL formula for the purposes of checking compliance along all paths. The examples.py file includes methods for running examples of this project's capabilities.

### Dependencies

This code entails the following dependencies: numpy, igraph, cvxpy, joblib, tqdm, pymdptoolbox.
* igraph (https://igraph.org/python/) is used for graph operations.
* cvxpy (https://www.cvxpy.org/) is used to solve convex optimization problems.
* joblib (https://joblib.readthedocs.io) is used for parallelization.
* tqdm (https://pypi.org/project/tqdm/) adds a CLI progress bar.
* pymdptoolbox (https://pymdptoolbox.readthedocs.io) is used to solve markov decision processes.

This code also relies on the nuXmv model checker (https://es-static.fbk.eu/tools/nuxmv/).
