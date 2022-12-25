#!/usr/bin/python3
"""
Factorize set of numbers in a file to give product of two smaller numbers"""
from sys import argv


def factorize(number):
    """ Multiply two smaller numbers to give desired number"""
    n = 2
    if number < 2:
        return
    while number % n:
        n += 1
    print("{:.0f}={:.0f}*{:.0f}".format(number, number // n, n))


if len(argv) != 2:
    exit()

try:
    with open(argv[1]) as file:
        line = file.readline()

        while line != "":
            number = int(line.split('\n')[0])
            factorize(number)
            line = file.readline()
except Exception:
    pass
