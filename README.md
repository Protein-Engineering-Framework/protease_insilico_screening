# protease_insilico_screening

This repository contains the source files and supplementary information for the the in silico-guided directed evolution of protease framework, which is described in Martin J. Thiele1§, Gaurao V. Dhoke1§, Felix Esser1, Isabell Hofmann1, Ulrich Schwaneberg1,2, Mehdi D. Davari*3, An In Silico-Guided Directed Evolution of Protease: Spotlighting the Beneficial Positions, To be published

## dock_batch_suc_Del_v4.svl
The svl file contains the code nessasary to repliacte the docking results reported in the paper. 
It requires a mdb file (*-rec*) with receptors to which molecules in a second mdb (*-lig*) are docked. 

*-m* determines how receptor side chains nearby the ligand are treated. ['Free', 'Fixed']

*-k* sets the strength of the pharmacophore constrains.

*-p* sets the maximum number of poses to retain.

*-o* Filename for the output mdb.

It features hardcoded pharmacophore constrains (lines 46-72) for the Subtilisin BL variant and the ligand Suc-AAPF-pNA used in the publication.

## SSM_v2.mdb
Contains the Subtilisin BL variants to which the ligand is docked (termed receptor in the svl), should be provided to the *-rec* option.

## Suc-AAPF-pNA_rebuild_Cov.mdb
Contains a single Suc-AAPF-pNA molecule (refered to as ligand) which is docked to the receptors in *SSM_v2.mdb*, should be provided to the *-lig* option.

## docking results
**still missing**