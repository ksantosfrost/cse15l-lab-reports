Failure Inducing Input and JUnitTest:

''' 
import org.junit.Test;
import static org.junit.Assert.*;

public class LinkedListTest {

    @Test(expected = NoSuchElementException.class)
    public void testLastEmptyList() {
        LinkedList list = new LinkedList();
        list.last();
    }
}


'''
