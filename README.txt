NAME: Christopher Nies
ID: A11393577
LOGIN: cs12sfl

DESCRIPTION OF PROGRAM:
MyLinkedList is my own personal implementation of the LinkedList data structure. It uses sentinel nodes to keep the implementation of the LinkedList methods simple, and also provides the methods to return an iterator that can iterate through the list.

TESTS:
These unit tests can be found in the MyLinkedListTester.java. I will briefly go over each one.

testGetHead()
The head that this test is testing is not the “head” instance variable in MyLinkedList, but rather simply the first element in the list. In the process it tests the “get” method, and the “add” method used to set up the linked list

testSet()
This test checks the “set” method at a specific index, with a specific element, and checks to make sure the element was set correctly.

testEmpty()
Tests to make sure that, in every circumstance, an empty list will return true when the isEmpty method is invoked and that a list that contains elements will not.

testIterator()
Tests an iterator to make sure that the next, and hasNext, methods are working correctly (at least in the sense that it does indeed iterate through the entire list and then stop.

testGetException()
This tests makes sure the proper exception is thrown in the “get” method, meaning in this case an “IndexOutOfBounds” exception.

testIteratorFibonacci()
Tests a very specific list that tests the add method, and the list’s ability to be traversed and checked against certain specific values. Essentially it tests how a user of this ADT could be using it

testAdd()
Tests the single argument “add” method to be sure that the element is correctly added to the end of the list, and that the list is correctly resized

testIteratorNext()
This test more thoroughly tests the iterator’s add method, including the fact that an exception should be thrown at the end of the file

testIteratorPrevious()
Same as above, only now moving backwards through the list

testIteratorHasNext()
Tests the iterator’s hasNext method in conjunction with the previous and add methods, as opposed to on it’s own

testIteratorIndex()
This test tests the “nextIndex” and “previousIndex” methods to see if they return the correct values of the element in the list

testIteratorHasPrevious()
Tests hasPrevious in conjunction with “previous” and “previousIndex” methods

testIteratorSet()
This is a thorough test of the Iterator’s set method, testing that the set method only adjusts a value if there was a call to next, and that the method throws an exception otherwise.

testRemove()
Test the list’s remove method, including the exception it throws when a user enters an invalid index.

testReturns()
Tests that the list’s “set” and “remove” methods return the correct values

testClear()
Tests the list’s “clear” method making sure that it resizes the list accordingly

KNOWN PROBLEMS OR ASSUMPTIONS:
While there are no problems with how the MyLinkedList functions, how it’s implemented is in my opinion unclean at times, such as with the iterator’s remove method reusing a lot of code that could have been its own helper method. Also, this implementation does not cover the case where an iterator is used to iterate through the list, but this list is modified using one of it’s methods (add, remove, etc.) versus the iterator’s. If this occurs, this list would be kind of broken due to the iterator’s left and right position possibly being messed, but Piazza said not to worry about it. However, it is then my assumption that the user, when iterating through the list with the iterator, will only modify the list using that iterator, and not with the list’s own methods. 
