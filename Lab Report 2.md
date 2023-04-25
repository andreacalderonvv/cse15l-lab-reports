## Lab Report 2

Part 1:
---
This is my String server code.

![Image](PART1p1)


Screenshot 1:

![Image](PART1p2)

In this screenshot, first the main method was called in order to get a port number. After handleRequest is called. If /add-message is used in the URL, then
the message in the query gets appended and is shown on the site. In the main method, the only relevant agrument is `String [] args` which ends up being the 
which port number is used. For `handleRequest`a `URI url` argument is taken in. From that arugment parts of it are taken and analzyed. For example the path and
then the query, in order to display the proper message on the server. In this screenshot, the values of `message`, a field meant to keep the strings on the server, are "test." `message` gets updated everytime /add-message is used. For the main method, args only contains the port number 4000.


Screenshot 2:

![Image](PART1p3)

In this screenshot, the main method is again called for the port number. The port number is taken in from the agrument `String [] args`.`handleRequest` is called too. It takes in the argument `URI url`. When /add-message is used in the URL a message gets appended. In this picture it was used three times for "hi", "hello", and "YASSSSS." In this program, the field `message` gets updated each time /add-message is used. `message` went from 

"hi"


to then;


"hi

hello"


and finally


"hi

hello

YASSSSS"


Part 2:
---
```
@Test 
	public void testReverseInPlace2() {
    int[] input1 = {1,2,3,4};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{4,3,2,1}, input1);
	}

```

pic here

failure inducing input

Part 3:
---
In week 2, I learned a lot about web servers. For example, before I knew nothing about how the code for web servers would look like.
After this lab,
