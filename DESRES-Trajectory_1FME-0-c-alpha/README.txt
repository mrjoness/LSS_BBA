                          1FME-0 Trajectory
                         D. E. Shaw Research
                           December 1, 2011
                                   
First of two independent simulations of the reversible folding of BBA
at 325K (see page 21 of the supplementary materials Lindorff-Larsen et
al., Science, 2011).

The suffix of the distribution directory's name encodes the selection
of frames from the full trajectory dataset:

  -all     : all frames, all atoms
  -protein : all frames, protein atoms only
  -c-alpha : all frames, alpha carbon atoms only

Each distribution directory contains a README.txt file, a
sub-directory containing DCD files, a structure file in Maestro
format, and a copy of the license file.  The DCD directory 1FME-0
contains segments of the trajectory 1FME-0-nnn.dcd in DCD form.  The
start time in picoseconds for each DCD segment is given in the
1FME-0/1FME-0_times.csv file, a comma separated value file that is
both human readable and spreadsheet compatible.  The system.mae file
contains the structure information used in the simulation.  There is
also a reduced structure file in the DCD directory that can be
different from the simulation structure file; for example, the reduced
structure file for trajectories consisting of only protein atoms,
contains only the appropriate atoms.

License
=======

The 1FME-0 trajectory dataset is released under the D. E. Shaw
Research Trajectory Data License Agreement a copy of which is
contained in the file DESRES_Trajectory_License.txt provided in this
distribution.

Citation
========

The use of any trajectory data in any reports or publications of
results obtained with the trajectory data should be acknowledged by
including a citation to the following paper:

  Kresten Lindorff-Larsen, Stefano Piana, Ron O. Dror, and David
  E. Shaw, "How Fast-Folding Proteins Fold," Science, vol. 334,
  no. 6055, 2011, pp. 517-520.

Viewing in VMD
==============

This trajectory may be viewed using the VMD version 1.8.7 or later (or
any other tool capable of reading files in DCD and Maestro format).
The VMD software is available from the Theoretical and Computational
Biophysics Group at the University of Illinois at Urbana-Champaign,
http://www.ks.uiuc.edu/Research/vmd

  Humphrey, W., Dalke, A. and Schulten, K., "VMD - Visual Molecular
  Dynamics", J. Molec. Graphics, 1996, vol. 14, pp. 33-38.

To view the full trajectory, change to the unpacked trajectory
directory and use the command:

  $ vmd 1FME-0/1FME-0/*.mae 1FME-0/1FME-0-*.dcd

Depending on the number of frames in the dataset, and the amount of
memory on your system, you might need to pass only a subset of the DCD
files on the command line.
