

garbage collection of str and num are late or we can say it is perpously gitve time because this optimse the performance 


code : (the reference is change in between that is why output is changed)

    >>> l1 = [1,2,3]
    >>> l2 = l1
    >>> l1
    [1, 2, 3]
    >>> l2
    [1, 2, 3]
    >>> l2 = [1,2,3]
    >>> l2
    [1, 2, 3]
    >>> l1[0] = 22
    >>> l1
    [22, 2, 3]
    >>> l2
    [1, 2, 3]
    >>> 

code : (because of same reference it is same)

    >>> p1 = [1,2,3]
    >>> p2 = p1
    >>> p1
    [1, 2, 3]
    >>> p2
    [1, 2, 3]
    >>> p1[0] = 33
    >>> p1
    [33, 2, 3]
    >>> p2
    [33, 2, 3]
    >>> 

code : (it will make a copy because of slicing)

    >>> a1 = [1,2,3]
    >>> a2 = a1[:]
    >>> a1
    [1, 2, 3]
    >>> a2
    [1, 2, 3]
    >>> a1[0] = 44
    >>> a1
    [44, 2, 3]
    >>> a2
    [1, 2, 3]
    >>> 


code : (`is` check inside the memory they have same refference or not)

    >>> t1 = [1,2,3]
    >>> t2 = [1,2,3]
    >>> t1 == t2
    True
    >>> t1 is t2 
    False
    >>> 