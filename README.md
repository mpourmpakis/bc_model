# bc_model_nanolett
This work is written and used in conjection with our work published in Nanoletters.
The paper can be found here: https://pubs.acs.org/doi/10.1021/acs.nanolett.8b00670
If you use the code please cite our paper!

To run these codes you will need access to Python 2.7 and the Atomic Simulation Environment (ASE)
Python 2.7: https://www.python.org/download/releases/2.7.4/
ASE: https://wiki.fysik.dtu.dk/ase/

We have written the codes to be command-line executable, so a linux operating system is recommended.

The basic workflow for these codes is as follows

1. Run '< ./CNS {}.xyz >' to generate the coordination number file '{}_cns.xyz'

2. Run '< ./BC_SRB_Model {}_cns.xyz >' on the newly generated CNS file to calculate the BC/SRB model Cohesive Energies 
