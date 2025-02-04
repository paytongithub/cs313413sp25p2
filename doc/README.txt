COMP 313/413 Project 2 Report

TestList.java and TestIterator.java

	TODO also try with a LinkedList - does it make any difference?

		Changing to a linked list makes no differences for the tests ran. It still runs and passes all tests as expected
        However, it does require another library import to work

TestList.java

	testRemoveObject()

		list.remove(5); // TODO Question: what does this method do?

		    list.remove(5) removes the value at the fifth index, in this case 77


		list.remove(Integer.valueOf(5)); // TODO Question: what does this one do?

			list.remove(Integer.valueOf(5)) searches the list and removes all value 5's


TestIterator.java

	testRemove()

		i.remove(); // TODO Question: what happens if you use list.remove(Integer.valueOf(77))?

			list.remove(Integer.valueOf(77)) removes all values of 77 right away, so when iterating, it breaks





TestPerformance.java

	State how many times the tests were executed for each SIZE (10, 100, 1000 and 10000)
	to get the running time in milliseconds and how the test running times were recorded.
	These are examples of SIZEs you might choose, you can choose others if you wish.

	SIZE 10
								  #1   #2   #3   #4   #5   #6
        testArrayListAddRemove:  879  833  794  866  845  808  ms
        testLinkedListAddRemove: 852  853  1000 925  854  828  ms
		testArrayListAccess:     784  801  872  857  819  816  ms
        testLinkedListAccess:    746  901  814  831  844  802  ms

	SIZE 100
								  #1   #2   #3   #4   #5   #6
        testArrayListAddRemove:  833  785  839  885  855  835  ms
        testLinkedListAddRemove: 843  934  819  873  829  834  ms
		testArrayListAccess:     828  792  817  764  797  856  ms
        testLinkedListAccess:    999  808  775  830  810  858  ms

	SIZE 1000
								  #1   #2   #3   #4   #5   #6
        testArrayListAddRemove:  1000 1000 1000 1000 1000 1000 ms
        testLinkedListAddRemove: 833  829  856  857  851  806  ms
		testArrayListAccess:     801  827  815  831  824  773  ms
        testLinkedListAccess:    1000 1000 1000 1000 1000 1000 ms

	SIZE 10000
								  #1   #2   #3   #4   #5   #6
        testArrayListAddRemove:  3000 3000 3000 3000 3000 3000 ms
        testLinkedListAddRemove: 918  894  857  898  883  880  ms
		testArrayListAccess:     843  993  836  833  810  838  ms
        testLinkedListAccess:    5000 4000 5000 4000 5000 4000 ms

	listAccess - which type of List is better to use, and why?

		For listAccess, as the SIZE increased, Linked List access stayed consistently quick,
		while the Array List took more and more time. Therefore, the Linked List is better


	listAddRemove - which type of List is better to use, and why?

		For listAddRemove, as SIZE increased, Array Lists stayed similarly consistent in its times,
		but Linked List took significantly more time as it it increased. Therefore, the Array List is better