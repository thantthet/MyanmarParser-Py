# MyanmarParser-Py

This is the python version of https://github.com/thanlwinsoft/MyanmarParser

## Usage

```python
m = MyParser()

str = u'နေကောင်းရဲ့လား'
offset = 0 

while offset < len(str):
	breaktype, next_offset = m.get_next_syllable(str, len(str), offset) # parse
	print str[offset:next_offset] # extract syllable using start offset and end offset
	offset = next_offset
	
# prints
# နေ
# ကောင်း
# ရဲ့
# လား
```
