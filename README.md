# 5practical-
import matplotlib.pyplot as plt
import seaborn as sns
import matplotlib as mpl
import matplotlib.pylab as pylab
import numpy as np
%matplotlib inline

import re

sentences="""My name is ashu. I am a very cute girl.I belong to a nuclear family.I am studying in final year"""


sentences=re.sub('[^A-Za-z0-9]+',' ',sentences)
print(sentences)


sentences=re.sub(r'(?:^| )\w(?:$| )', '',sentences).strip()
print(sentences)

sentences=sentences.lower()

print(sentences)

data=[]
for i in range(2,len(words)-2):
  context=[words[i-2],words[i-1],words[i+2]]
  target=words[i]
  data.append((context,target))
  print(data[5:])
