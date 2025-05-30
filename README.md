# dir\_to\_df
Manage a corpus of filepaths and metadata as a Pandas DataFrame created from a directory tree.

## Examples

```
from dir_to_df import dir_to_df

# Get all files in `mypath`
df = dir_to_df(mypath)

# Get all `.wav` files in `mypath`
df = dir_to_df(mypath, fnpat=r'\.wav$')

# Get all `.wav` files in `mypath` and extract named captures for files named like CC12-47.wav
df = dir_to_df(mypath, fnpat=r'(?P<subj>[A-Z]+\d+)-(?P<token>\d+)\.wav$')
```

