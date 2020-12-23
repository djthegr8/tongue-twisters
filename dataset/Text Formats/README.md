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
*TODO*
