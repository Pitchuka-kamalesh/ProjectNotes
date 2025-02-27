# ProjectNotes
It's used to help me to write all the project related nodes in one place

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
