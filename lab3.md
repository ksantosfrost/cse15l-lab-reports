Failure Inducing Input and JUnitTest:

```java
import org.junit.Test;
import static org.junit.Assert.*;
import java.util.NoSuchElementException;

public class LinkedListTest {

    @Test(expected = NoSuchElementException.class)
    public void testFirstOnEmptyList() {
        LinkedList list = new LinkedList();
        list.first(); 
    }
}
```

Input that does not induce a failure and JunitTest:

```java
import org.junit.Test;
import static org.junit.Assert.*;
import java.util.NoSuchElementException;

public class LinkedListTest {
 @Test
    public void testLengthAfterInsertions() {
        LinkedList list = new LinkedList();
        list.prepend(10);
        list.append(20);  
        list.prepend(30); 
        assertEquals("List should have 3 elements", 3, list.length());
    }
}
```
![Code](lab3ss/code1.PNG)

Fix/Bug
```java
public int first() {
    if (this.root == null) {
        throw new NoSuchElementException("Cannot access first element on an empty list.");
    }
    return this.root.value;
}
```
The first() method is supposed to return the value of the first element in the list. If the list is empty, it should throw a NoSuchElementException. The implementation does not handle the case if the list is empty. With this change I made, it checks if the root is null before trying to return the value. if it is null, it throws a NoSuchElementException which is the expected behavior when trying to access the first element of an empty list.

**Command find**

Example -name 1:
```bash
find ./technical -name ".txt"
```
The -name option allows you to search for files whose name matches a pattern. This command looks for all files that end with ".txt" in the ./technical directory.

Output:

![-name](lab3ss/-nameexample.PNG)

Example -name 2:

```bash
find ./technical -name "report.docx"
```
This command searches for a file named report.docx in the ./technical directory. 
