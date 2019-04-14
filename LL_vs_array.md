Linked Lists vs Arrays

-LL have faster insertions and deletions
    -find place
    -store next node
    -set pointer from previous to new
    -set pointer from new to oldNew
    -O(1)

-LL require no size declaration (memory allocation)

-LL take extra size memory; must store data and pointers

-LL have slower search
    -even if you know where the data is that you want, you still have to start from the beginning until you find that data
    -head -> data -> data -> *data* -> more

    -arrays have O(1) time complexity for searching if you know the index.  

    -LL have 0(n) time complexity, since the node you're searching for may be the last item in the list




