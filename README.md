# bc_model
This work is written and used in conjection with our work published in Nanoletters.
The paper can be found here: https://pubs.acs.org/doi/10.1021/acs.nanolett.8b00670
If you use the code please cite our paper!

1. Yan, Z.; Taylor, M. G.; Mascareno, A.; Mpourmpakis, G. "Size-, Shape-, and Composition-Dependent Model for Metal Nanoparticle Stability Prediction" Nano Lett. 2018, 18 (4), 2696–2704.

To run these codes you will need access to Python 2.7 and the Atomic Simulation Environment (ASE)
Python 2.7: https://www.python.org/download/releases/2.7.4/
ASE: https://wiki.fysik.dtu.dk/ase/

We have written the codes to be command-line executable, so a linux operating system is recommended.

The basic workflow for these codes is as follows

1. Run '< ./CNS {}.xyz >' to generate the coordination number file '{}_cns.xyz'

2. Run '< ./BC_SRB_Model {}_cns.xyz >' on the newly generated CNS file to calculate the BC/SRB model Cohesive Energies 

The Files are as follows:

BC_SRB_Model - python code that takes in a modified .xyz file and evaluates the BC/SRB model Cohesive Energy

CNS - python code that takes in a regular .xyz file and generates coordination numbers (CNS) and bonding topologies for a given MNP structure and generates a modified .xyz file with this information

EE_analysisFePt - python code used to analyze the excess energy of the large FePt nanoalloy used in Yang et al. Nature 2017, 542, 75-70

FePt_cns_final.xyz - modified .xyz file with CNS and bonding topology as an example of the output from the CNS code and for use in the EE_analysisFePt code

WF_refer_1.csv - csv file containing the data used in the BC model for the dimer binding energy weight factors (Primary Source)

WF_refer_2.csv - csv file containing secondary data for use in the BC model for the dimer binding energy weight factors
