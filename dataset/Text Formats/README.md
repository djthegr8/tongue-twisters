## Text formats
This dataset is available in two text formats, namely ~
* [TXT](./database.txt)
* [CSV](./database.csv)
                               
The usage of both these files is simple.       
#### 1. TXT File
To use this, simply import it into your workspace, script or Jupyter notebook, which may look like the below in Python.
```py
tongue_twisters_str = open('../input/tongue-twister-dataset/database.txt', 'rb').read().decode(encoding='utf-8')
```
After that's done, to get the examples as an array, split the string by the `|` (a.k.a pipe) symbol, like 
```py
tongue_twisters = tongue_twisters_str.split('|')
```
Done 🎉 You're good to go!                          
#### 2. CSV File
we have created the CSV file with all the different examples in rows.               
Thus, using it would look like the below.
```py
# Using Pandas, as it is very commonly used for Data Science
import pandas as pd
# Simply importing it as a pandas DataFrame
tongue_twister = pd.read_csv(
                             "https://raw.githubusercontent.com/djthegr8/tongue-twisters/main/dataset/Text%20Formats/database.csv",
                             header=None,
                             )[0].to_frame()
# To see the first few tongue twisters
tongue_twister.head()
```
