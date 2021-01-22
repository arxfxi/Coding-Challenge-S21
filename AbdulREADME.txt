//ABDUL RAFAI SUBMISSION

#INSTRUCTIONS 
1. Just open this link or open ipynb file in github branch
https://colab.research.google.com/drive/10k73JyStPwSfTL_5jXOlfnwvFc_qdhcb?usp=sharing

#If doesn't work/show you may run it yourself
1. DOWNLOAD genomeProjAbdul.ipynb file 
2. Run in Google Colab - Must be in Chrome

3. Run cells - One cell will pop up a button called Choose Files and simply
choose Genome.gb from computer

4. Everything else should run smoothly and last png is the one uploaded.

Libraries used - 
!pip install ReportLab
!pip install biopython
from reportlab.lib import colors
from reportlab.lib.units import cm
from Bio.Graphics import GenomeDiagram
from Bio import SeqIO
import pandas as pd
import requests
from IPython.core.display import Image
from google.colab import files

//Will all work by themselves as long as in google colab

#EXPLANATION
A genbank file contains DNA info, protein sequences, and feaures of certain genes.
Usually these are plotted linearly, like bar graphs, and while that provides
solid info, a circular genome plot allows us to see relations and proximities 
between certain features in the virus. 
Therefore using Python, we can extract the gene features from the genbank plot,
look at its positions (relative to the other features) and plot it. We can also label
these features because their names are in the genBank file. This ends in a final plot
that shows distinct regions of the features, with their labels, and in some complex organisms,
allows us to more easily understand proximitiy of genome features.
