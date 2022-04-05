def fib(n):              
    if n == 1:
        result = 1
    elif n == 2:
        result = 2
    else:
        result = fib(n-1) + fib(n-2)
    return result

print(fib(4))