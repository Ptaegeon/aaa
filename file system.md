---
# 1 line save

```python
def line_reader(file_path):
  with open(file_path, 'r') as source_file:
    for line in source_file:
      yield line
      

reader = line_reader('big-data.txt')

with open('big-data-corrected.txt', 'w') as target_file:
  for line in reader
    taraget_file.wirte(line)
```
***

# chunk save
```python
with open('abc.jpg', 'rb') as source_file:
  while True:
    chunk = source_file.read(1024)
    if chunk :
      process_data(chunk)
      
    else:
      break
```
