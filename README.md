# python  

open
```
# txt  
lines = open('path.txt').readlines()  

# pickle  
pickle.dump(val_dict, open('path.pickle', 'wb'), protocol=pickle.HIGHEST_PROTOCOL)
load_dict = pickle.load(open('path.pickle', 'rb'))
```   

find all text  
```
[n for (n, e) in enumerate(text) if e == '/']
```
