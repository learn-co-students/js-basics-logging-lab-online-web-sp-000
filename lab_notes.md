**Lab Notes**

# Why Spies?
Open up the test/indexTest.js file

Learn why you are using this feature.

Underneath the code:

describe('console.log', function () { ..., you can see the code spy = sinon.spy(console, 'log');.

This asks your tests to watch the console.log function.

Later on in an it block...
you can ensure that console.log is called,
and can see what arguments it is called with.

You are using the spy because there really is no other great way to test the use of console.log.

The function returns undefined, so you can't really check the return value of your code, and console.log affects your browser's console, which humans can read easily,
but computers can't.

Test to make sure you made use of this function using a spy.
