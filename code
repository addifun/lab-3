import sys

def find_pairs(numbers):
    pairs = []
    seen = set()

    for num in numbers:
        complement = 10 - num
        if complement in seen:
            pair = (complement, num)
            pairs.append(pair)
        seen.add(num)

    return pairs

if __name__ == "__main__":
    numbers = [int(num) for num in sys.argv[1:]]
    pairs = find_pairs(numbers)

    for pair in pairs:
        print(pair[0], "+", pair[1])
