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
then the query, in order to display the proper message on the server. In this screenshot, the values of `message`, a field meant to keep the strings on the server, are "test test." `message` gets updated everytime /add-message is used. For the main method, args only contains the port number 4000.


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
In this part, we will be looking at some bugs from Lab 3. The bug I chose is from ArrayExamples.java in the method `reversed`.

**This is failure input.**

```
@Test
  public void testReversed3() {
    int[] input1 = {3};
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```

**This is non-failure producing input.**

```
@Test
  public void testReversed2() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```

**Symptom of failure input.**

![Image](failure)

**Symptom of non-failure input.**

![Image](nonfailure)

**Code Before**

```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```

**Code After**
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
 What I did to fix this issue was that I noticed that `arr[i] = newArray[arr.length - i - 1];` was assigning the new empty array to the old array in reverse.
 Since there was nothing in the new Array, it was simply assigning 0's to the old array. What I did was change the line to 
 `newArray[i] = arr[arr.length - i - 1];`. This line now assigns the old values of array `arr` to `newArray` in reverse order. This fixes the issue of just 
 assigning zeros to the old array. I also changed the return statement to return `newArray` instead of `arr`.

Part 3:
---
In lab 2, I learned a lot about web servers. For example, before I knew nothing about how the code for web servers would look like. It was fun to see how it handled paths and queries. After this lab, I also learned about the different parts of a URL. For example, what a query does and how it can take in information. It was really interesting to see how everything worked.
