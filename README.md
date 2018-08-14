# Cube

************************************************************************************************************************
 Basic understanding of .mtl File in OpenGl
("Source : https://en.wikipedia.org/wiki/Wavefront_.obj_file")

************************************************************************************************************************


 >>> .Mtl File Normalization 


A single .mtl file may define multiple materials. Materials are defined one after another in the file, each starting with the newmtl command:

# define a material named 'Colored'
   newmtl Colored

The ambient color of the material is declared using Ka. Color definitions are in RGB where each channel's value is between 0 and 1.
Ka 1.000 1.000 1.000     # white

Similarly, the diffuse color is declared using Kd.
Kd 1.000 1.000 1.000     # white


The specular color is declared using Ks, and weighted using the specular exponent Ns.
Ks 0.000 0.000 0.000     # black (off)
Ns 10.000                # ranges between 0 and 1000

understanding of this three Light Color
https://qph.ec.quoracdn.net/main-qimg-dbc0172ecc9127a3a6b36c4d7f634277.webp


Materials can be transparent. This is referred to as being dissolved. Unlike real transparency, the result does not depend upon the thickness of the object. A value of 1.0 for "d" is the default and means fully opaque, as does a value of 0.0 for "Tr".

d 0.9                    # some implementations use 'd'
   Tr 0.1                   # others use 'Tr' (inverted: Tr = 1 - d)
 
 
 
   
