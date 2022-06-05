### An exmaple how to detect Palindrome or Symmetrica strings in given text or string 
## this an exmaple implemented with recursive function with python code
```python
a="find Palindrome or Symmetrica in any given text like momkljhhamomallaboba"

def detect(text):
    if len(text) > 2:
      if text == text[::-1]:
        print(text)
        return 
      else: 
        for i in range(len(text)-2):
          if text[:-i-1] == text[:-i-1][::-1]:
            print(text[:-i-1]) 
            detect(text[-i-1:])
            return
        detect(text[1:])
    else:
       return 
detect(a)
```

# output:
```bash
mm
mom
hh
amoma
ll
aboba
```
