# python  

open
```
# txt  
open('readme.txt', 'w') .writelines(lines)
lines = open('path.txt').readlines()  

# pickle  
pickle.dump(val_dict, open('path.pickle', 'wb'), protocol=pickle.HIGHEST_PROTOCOL)
load_dict = pickle.load(open('path.pickle', 'rb'))
```   

text slicing
```
[n for (n, e) in enumerate(text) if e == '/']
```

```
from fastai.vision.all import Path
[i for i in list(Path(directory).rglob('*.JPEG')) if 'ipynb' not in str(i)]
```


```
import wget
import math

def bar_custom(current, total, width=80):
    width=30
    avail_dots = width-2
    shaded_dots = int(math.floor(float(current) / total * avail_dots))
    percent_bar = '[' + '■'*shaded_dots + ' '*(avail_dots-shaded_dots) + ']'
    progress = "%d%% %s [%d / %d]" % (current / total * 100, percent_bar, current, total)
    return progress
    
wget.download(classifier, out = '/home/lhj/diffusion_dataset', bar=bar_custom)
```
