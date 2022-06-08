## IS number is prime :
```python
def is_prime(Num):
    Until = int(Num**0.5)+1
    for n in range(2,Until):
        if Num%n==0:
            return False
    return True  

is_prime(307)
output : True
```

## find the prime in location N 
# Recursive :
```python 
def find_n_prime(i,N):
    if N == 0 :
        return
    else:
        if is_prime(i):
            global  prime 
            prime = i 
            find_n_prime(i+1,N-1)
        else:
          find_n_prime(i+1,N)
find_n_prime(1,200)
output:1217
```
# loop method
```python 
def find_the_N_prime(N):
  i = 1
  while N > 0 :
    if is_prime(i):
        prime = i 
        N -= 1
    i += 1
  return prime  
find_the_N_prime(500)
output: 3559
```
