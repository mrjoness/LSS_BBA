# LSS Applied to DEShaw simulations of the BBA (PDB: 1FME)

The collab notebook loads the Ca positions of BBA simulations with stride=50 and three pre-trained models for the SRV, MDN, and DDPM. Walkthrough includes analysis of implied timescales, eigenvector correlations with input features, and differences in metastable states.

### SRV:
- Trained on 10 x 100_000 trajectories of BBA with lag=50
- Features are all pairwise distances between Ca positions
- Analysis shows correlations to input features and differentiates metastable states

### MDN:
- Trained on the 6 leading eigenvectors learned by the SRV with lag=50
- Reproduces the thermodynamics and transition kinetics of training data

### DDPM:
- Trained to reconstruct the Ca positions conditioned on a coordinate in SRV space
- Uses a 1000-step diffusion process guided by coordinate space
