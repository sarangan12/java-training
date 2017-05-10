## What is the difference between String, StringBuffer and StringBuilder?
String, StringBuffer and StringBuilder are 3 different classes in Java. String class is immutable i.e. If a String object is created, the value of the object could not be modified. But, if the scenario warrants a lot of modifications to a String, then in order to accomodate such scenarios, We use StringBuffer or StringBuilder classes. 

## What do you mean by "String is immutable"?
 If a String object is created, the value of the object could not be modified. For eg:

```
 String str = "Sample"
 str =  "xyz"
```

In the above code, first an object is created with value "Sample". Then, instead of modifying the value of that object, a new object with value 'xyz' is created and str points to the new object. Thus the value of the string object cannot be modified after creation i.e. immutable. 

## How does the StringBuffer/StringBuilder classes become mutable?
Let us take an example:

```
 StringBuffer buffer = new StringBuffer();
 buffer.append("Sample");
 buffer.append("xyz");
 String str = buffer.toString();
```

In the above code, there is only one StringBuffer object is created and the value of that object is initially empty. Then, the values "Sample" and "xyz" are appended to the same object. 

## Why is String made immutable? 
String object are common objects in programming. In multithreaded programming scenarios, we do not want threads making accidental changes to the Strings. Thus, String objects are made immutable. 

## What is the difference between StringBuffer and StringBuilder? 
The functionality provided by the StringBuffer & StringBuilder classes are identical. But, StringBuffer is thread safe i.e. it can be used safely in multithreaded programming. Whereas, StringBuilder class is not thread safe. As a result, StringBuilder is much faster (because it is not thread safe) than StringBuffer.

## What is a StringTokenizer class? 
StringTokenizer is a class that is used to split the Strings into multiple tokens.

## What is the difference between StringTokenizer class and Split method? 
StringTokenizer class is a legacy class which exists for compatability reasons. The Split method exists as part of String class and currently recommended approach to Split the strings. 