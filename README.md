

Schoeberl2002 - EGF MAPK

Computational model that offers an integrated quantitative, dynamic, and
topological representation of intracellular signal networks, based on known
components of epidermal growth factor (EGF) receptor signal pathways.

The initial model was constructed by Ken Lau from the [MATLAB source
code](http://web.mit.edu/dllaz/egf_pap/).

This model is described in the article:

[Computational modeling of the dynamics of the MAP kinase cascade activated by
surface and internalized EGF
receptors.](http://identifiers.org/pubmed/11923843)

Schoeberl B, Eichler-Jonsson C, Gilles ED, Müller G

Nat. Biotechnol. 2002 Apr; 20(4): 370-375

Abstract:

We present a computational model that offers an integrated quantitative,
dynamic, and topological representation of intracellular signal networks,
based on known components of epidermal growth factor (EGF) receptor signal
pathways. The model provides insight into signal-response relationships
between the binding of EGF to its receptor at the cell surface and the
activation of downstream proteins in the signaling cascade. It shows that EGF-
induced responses are remarkably stable over a 100-fold range of ligand
concentration and that the critical parameter in determining signal efficacy
is the initial velocity of receptor activation. The predictions of the model
agree well with experimental analysis of the effect of EGF on two downstream
responses, phosphorylation of ERK-1/2 and expression of the target gene,
c-fos.

This model does **not** exactly reproduce the results given in the original
publication. It has, though, the same reaction graph and gives very similar
time courses for the conditions depicted in the article.

Several corrections were applied to the parameters described in the paper's
supplementary materials. Some parameter names were replaced by the
corresponding identical ones: k(r)26 by k(r)18, k(r)27 by k(r)19, k(r)30 by
k(r)20, k(r)38 by k(r)24, k(r)39 by k(r)37, k(r)46 by k(r)44, k51 by k49,
k(r)54 by k(r)52 and k62 by k62. In particular the parameter values described
in the column "remark" of supplementary table 1 override the values
explicitely written in the numerical columns:

name | in suppl. value used | in model value used | remarks  
---|---|---|---  
kr16 | 0.055 | 0.275 |  
k30 | 7.9e6 | 2.1e6 | as k20  
kr30 | 0.3 | 0.4 | as kr24  
k38 | 3e7 | 1e7 | as k20  
kr38 | 0.055 | 0.55 | as kr24  
k52 | 1.1e5 | 5.34e7 |  
  
k5 was used for v116, v119, v122 and v125 in addition of v107, v110 and v113
as listed in the legend of supplementary figure 2. k5 is calculated using th
eformula from the matlab file not given in the supplements.

All rate constants were rescaled to minutes (k[min] = 60*k[sec]) and all
second order rate constants additionally to molecules/cell with a cell volume
of 1 picolitre (k[molecs/cell] = k[M]/(Vc*Na), with Vc=1e-12 l and Na = 6e23).

The association constant of internalized EGF was rescaled to
molecules/endosome using an endosomal volume of 4.3 al (= 4.3*10 -18 litre).

The extracellular EGF concentration was converted to molecules per picolitre
with a MW of 6045 Da.

[ng/ml] | [numb/pl]  
---|---  
50 | 4962  
0.5 | 49.6  
0.125 | 12.4  
  
With the initial conditions given in the paper, the results could not be
reproduced at all. Therefore the initial conditions used in the MATLAB file
were adopted for SHC (1.01 * 10 5 instead of 1.01 * 10 6 ) and Ras_GDP. (7.2 *
10 4 instead of 1.14 * 10 7 )

This model is hosted on [BioModels Database](http://www.ebi.ac.uk/biomodels/)
and identified by:
[BIOMD0000000019](http://identifiers.org/biomodels.db/BIOMD0000000019).

To cite BioModels Database, please use: [BioModels Database: An enhanced,
curated and annotated resource for published quantitative kinetic
models](http://identifiers.org/pubmed/20587024).

To the extent possible under law, all copyright and related or neighbouring
rights to this encoded model have been dedicated to the public domain
worldwide. Please refer to [CC0 Public Domain
Dedication](http://creativecommons.org/publicdomain/zero/1.0/) for more
information.

