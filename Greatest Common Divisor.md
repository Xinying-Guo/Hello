# python3
def gcd_naive(a,b):
    if a > b:
        m = a%b
        while m > 0:
            a = b
            b = m
            m = a%b
        return b
    else:
        m = b%a
        while m > 0:
            b = a
            a = m
            m = b%a
        return a
