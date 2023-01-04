---
layout: page
title: How to
permalink: /how_to/
---

### It's all about how to's

* python how to append at the beginning \
    # using insert() to append \
    # at beginning. append 6 \
    test_list.insert(0, 6) \
    [https://www.geeksforgeeks.org/python-perform-append-at-beginning-of-list/](https://www.geeksforgeeks.org/python-perform-append-at-beginning-of-list/)

* python max integer \
    import sys \
    max_size = sys.maxsize \
    min_size = -sys.maxsize - 1 \
    If you just need a number that's bigger than all others, you can use \
    float('inf') \
    in similar fashion, a number smaller than all others: \
    float('-inf') \
    [https://stackoverflow.com/questions/7604966/maximum-and-minimum-values-for-ints](https://stackoverflow.com/questions/7604966/maximum-and-minimum-values-for-ints)

* python initialize 2d array with zeros \
    for Python 3 (no more xrange), the preferred answer \
    zeros = [ [0] * N for _ in range(M)]  \
    for M x N array of zeros  \
    [https://stackoverflow.com/questions/13157961/2d-array-of-zeros](https://stackoverflow.com/questions/13157961/2d-array-of-zeros)


* python dictionary
    # Creating a Dictionary \
    # with dict() method \
    Dict = dict({1: 'Geeks', 2: 'For', 3: 'Geeks'}) \
    print("\nDictionary with the use of dict(): ") \
    print(Dict)
    
    # Creating a Dictionary \
    # with each item as a Pair \
    Dict = dict([(1, 'Geeks'), (2, 'For')])

    # Adding set of values \
    # to a single Key \
    Dict['Value_set'] = 2, 3, 4

    # Creating an empty Dictionary \
    Dict = {} \
    print("Empty Dictionary: ") \
    print(Dict)
    
    # Adding elements one at a time \
    Dict[0] = 'Geeks' \
    Dict[2] = 'For' \
    Dict[3] = 1 \
    print("\nDictionary after adding 3 elements: ") \
    print(Dict)
    
    # Adding set of values \
    # to a single Key \
    Dict['Value_set'] = 2, 3, 4 \
    print("\nDictionary after adding 3 elements: ") \
    print(Dict)
    
    # Updating existing Key's Value \
    Dict[2] = 'Welcome' \
    print("\nUpdated key value: ") \
    print(Dict)
    
    # Adding Nested Key value to Dictionary \
    Dict[5] = {'Nested': {'1': 'Life', '2': 'Geeks'}} \
    print("\nAdding a Nested Key: ") \
    print(Dict)

    Dictionary methods \
    clear() – Remove all the elements from the dictionary \
    copy() – Returns a copy of the dictionary \
    get() – Returns the value of specified key \
    items() – Returns a list containing a tuple for each key value pair \
    keys() – Returns a list containing dictionary’s keys \
    pop() – Remove the element with specified key \
    popitem() – Removes the last inserted key-value pair \
    update() – Updates dictionary with specified key-value pairs \
    values() – Returns a list of all the values of dictionary \
    [https://www.geeksforgeeks.org/python-dictionary/](https://www.geeksforgeeks.org/python-dictionary/)

* python unicode
    Python ord() function returns the Unicode code from a given character

* python hash set
    set() \
    add(), discard(), update(), union()
    [https://www.programiz.com/python-programming/set](https://www.programiz.com/python-programming/set)

* python sort list
    # function to return the second element of thec
    # two elements passed as the parameter \
    def sortSecond(val): \
        return val[1]
    
    # list1 to demonstrate the use of sorting \
    # using  second key \
    list1 = [(1, 2), (3, 3), (1, 1)] \
    
    # sorts the array in ascending according to \
    # second element \
    list1.sort(key=sortSecond) \
    print(list1)
    
    # sorts the array in descending according to \
    # second element \
    list1.sort(key=sortSecond, reverse=True) \
    print(list1)

    [https://www.geeksforgeeks.org/python-list-sort-method/](https://www.geeksforgeeks.org/python-list-sort-method/)
