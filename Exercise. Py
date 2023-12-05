import itertools

if __name__ == '__main__':
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())
    print([list(t) for t in itertools.product(
               range(x + 1), range(y + 1), range(z + 1))
           if sum(t) != n])
