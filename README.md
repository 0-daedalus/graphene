# README
Article title: Determining the structure of functionalized graphene for tailored thermomechanical properties using ML techniques.

Authors: Ravil Ashirmametov, Alexandr Alpatov, Farrokh Yousefi, Narges Vafa, Siamac Fazli and Konstantinos Kostas.

Corresponding author: Ravil Ashirmametov, ravil.ashirmametov@nu.edu.kz



Two datasets are uploaded in the /datasets:

File names are **Results\_for\_H.csv** for hydrogen case, and **Results\_for\_methyl.csv** for methyl case. Datasets are structured as follows:

8528 columns with integer encoding of the layout (1,2,3,4 integer values)

Four columns with extracted thermomechanical properties, in order:

1\. Kappa	

2\. Max Strain

3\. Max Stress

4\. Young's Modulus



For the 8528 columns representing the layout:

1 (both cases) - carbon atom without functionalization;

2 (hydrogen case) - carbon atom and top functionalization with hydrogen atom;

3 (hydrogen case) - carbon atom and bottom functionalization with hydrogen atom;

3 (methyl case) - carbon atom and top functionalization with methyl group;

4 (methyl case) - carbon atom and bottom functionalization with methyl group.



Two attached LAMMPS scripts are in the /LAMMPS Sample Scripts:

**sample\_mechanical** is a LAMMPS script used for MD simulation of the graphene for extraction of three targeted mechanical properties (Young's Modulus, maximum stress, strain at maximum stress);

**sample\_thermal** is a LAMMPS script used for MD simulation of the graphene for extraction thermal conductivity.



To go from the integer encoding in the datasets to a LAMMPS data file, we use following encoding strategy:
![Graphene Structure](./misc/graphenestructure.png)







