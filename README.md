# repo1
Program_Fitch_Solutions


Create a class or group of classes that does the following:

Accepts a request message that consists of 
	1.  a message string
	2.  a completion callback 
	3.  a message type (valid values: ['red', 'yellow', 'blue'])
	4.  a message priority (valid values: [1, 2, 3])

These messages should be stored.

Messages will be requested from an instance of the class by message type.  The instance should return the highest priority message of that type in FIFO order.  So, in order of evaluation, the returned message should be selected by
	1.  message type
	2.  message priority
	3.  message order
The selected message should be deleted from the store and the message string and completion callback should be returned to the callee.  


Your class should 
	* be thread-safe
	* validate input
	* handle errors
