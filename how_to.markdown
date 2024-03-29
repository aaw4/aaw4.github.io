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

* python string manipulation cheatsheet:
    and all other python cheat sheet included: \
    [https://www.pythoncheatsheet.org/cheatsheet/manipulating-strings](https://www.pythoncheatsheet.org/cheatsheet/manipulating-strings)

* python string to list
    [https://www.geeksforgeeks.org/python-program-convert-string-list/](https://www.geeksforgeeks.org/python-program-convert-string-list/)

* python list to string
    xs = ['1', '2', '3'] \
    s = ''.join(xs) \
    If the list contains integers, convert the elements to string before joining them:

    xs = [1, 2, 3] \
    s = ''.join(str(x) for x in xs)
    [https://stackoverflow.com/questions/5618878/how-to-convert-list-to-string](https://stackoverflow.com/questions/5618878/how-to-convert-list-to-string)

* python count specific character in a string
    counter = s.count(' ')

* python extend a list
    res.extend([' '] * counter * 2)

* python how to parse string to do calculation and return integer; formatting string
    python eval() function parses the expression argument and evaluates it as a python expression
    int(eval(f'{second_num} {item} {first_num}'))

* python heap
    # initializing list \
    li = [5, 7, 9, 1, 3]
    
    # using heapify to convert list into heap \
    heapq.heapify(li)

    # using heappush() to push elements into heap
    # pushes 4
    heapq.heappush(li, 4)
    
    # printing modified heap
    print("The modified heap after push is : ", end="")
    print(list(li))
    
    # using heappop() to pop smallest element
    print("The popped and smallest element is : ", end="")
    print(heapq.heappop(li))

    import heapq \
    listForTree = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15] \
    heapq.heapify(listForTree)             # for a min heap \
    heapq._heapify_max(listForTree)        # for a maxheap!! \
    If you then want to pop elements, use:

    heapq.heappop(minheap)      # pop from minheap \
    heapq._heappop_max(maxheap) # pop from maxheap

    (https://www.geeksforgeeks.org/heap-queue-or-heapq-in-python/)[https://www.geeksforgeeks.org/heap-queue-or-heapq-in-python/]

* python how to loop through a dictionary
    for state, capital in statesAndCapitals.items(): \
    print(state, ":", capital)

    for i in statesAndCapitals: \
    print(i, '->', statesAndCapitals[i])

    [https://www.geeksforgeeks.org/iterate-over-a-dictionary-in-python/](https://www.geeksforgeeks.org/iterate-over-a-dictionary-in-python/)

* python reverse list
    reversed(listobject)

* python check if a string start with 0
    {% highlight python %}
    string = "012345"
    if string.startswith("0"):
        print("The string starts with 0")
    else:
        print("The string does not start with 0")
    {% endhighlight %}

* python sort when there's a tie:
    people.sort(key=lambda x: (-x[0], x[1]))


* python calculate 1's and 0's in a string. for example, '11100110'
    {% highlight python%}
    string = '11100110'
    num_ones = string.count('1')
    num_zeros = string.count('0')
    {% endhighlight %}

