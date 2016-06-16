# Word-Word Co-occurence Matrix

Simple class for converting list of raw documents to co-ocurence matrix.


## Example

```python
import Cooccurence
docs = ['this book is good',
        'this cat is good',
        'cat is good shit']
model = Cooccurence(ngram_range=(1, 1), stop_words='english')
Xc = model.fit_transform(docs) # co-occurrence matrix

model.vocabulary_ # vocabulary
```


## Dependecies

- [scikit-learn](http://scikit-learn.org/stable/install.html)
