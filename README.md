# ProjectNotes
It's used to help me write all the project-related nodes in one place

#### Test annotation and its attributes 
```java
import org.testng.annotations.Test

@Test 
```
- alwaysRun  = false|true
  - default: false
  - >  /**
    > * If set to true, this test method will always be run even if it depends on a method that failed.
    > * This attribute will be ignored if this test doesn't depend on any method or group.
    > *
    > * @return the value (default false)
    > */
- priority = int  -ve|0|+ve
  - default: 0
    >   /**
    >  * The scheduling priority. Lower priorities will be scheduled first.
    >  *
    >  * @return the value (default 0)
    > */ 
- enabled = true/false
  - default: true
   >   /**
   > * Whether methods on this class/method are enabled.
   > *
   > * @return the value (default true)
   > */ 
- groups = { "functest", "checkintest" }
  - default: {}
  > The list of groups this class/method belongs to.
  > Returns:
  > the value

