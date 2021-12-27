#!/usr/bin/env python
# --------------------------------------------------------------------------------------------------------- Intermediate
import math; import random; import numpy as np; import io; from io import StringIO

def main():
    portnames = ["PAN", "AMS", "CAS", "NYC", "HEL"]

    port1 = 0
    for port2 in range(1, 5):
        for port3 in range(1, 5):
            for port4 in range(1, 5):
                for port5 in range(1, 5):
                    route = [port1, port2, port3, port4, port5]

                    # Modify this if statement to check if the route is valid
                    if port2 != port3 and port2 != port4 and port2 != port5 and port3 != port4 and port3 != port5 and port4 != port5:
                        # print(route)
                        # do not modify this print statement
                        print(' '.join([portnames[i] for i in route]))

main()

# --------------------------------------------------------------------------------------------------------- Advanced
portnames = ["PAN", "AMS", "CAS", "NYC", "HEL"]

def permutations(route, ports):
    if len(ports) < 1:
        print(' '.join([portnames[i] for i in route]))
        print(route)
    else:
        for i in range(len(ports)):
            permutations(route+[ports[i]], ports[:i]+ports[i+1:])
# This will start the recursion with 0 ("PAN") as the first stop
permutations([0], list(range(1, len(portnames))))
