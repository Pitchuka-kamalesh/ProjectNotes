# ProjectNotes

It's used to help me write all the project-related nodes in one place

#### Test annotation and its attributes

```java
import org.testng.annotations.Test

@Test 
```

- alwaysRun  = false|true
  - default: false
  - > /**
    > - If set to true, this test method will always be run even if it depends on a method that failed.
    > - This attribute will be ignored if this test doesn't depend on any method or group.
    > -
    > - @return the value (default false)
    > */
- priority = int  -ve|0|+ve
  - default: 0
    > /**
    > - The scheduling priority. Lower priorities will be scheduled first.
    > -
    > - @return the value (default 0)
    > */
- enabled = true/false
  - default: true
    > /**
    > - Whether methods on this class/method are enabled.
    > -
    > - @return the value (default true)
    > */
- groups = { "functest", "checkintest" }
  - default: {}
    > The list of groups this class/method belongs to.
    > Returns:
    > the value
- dependsOnGroups = {"functest"}
  - default: {}
    > The list of methods this method depends on. There is no guarantee on the order on which the methods depended upon will be run, but you are guaranteed that all these methods will be run before the test method that contains this annotation is run. Furthermore, if any of these methods was not a SUCCESS, this test method will not be run and will be flagged as a SKIP.
    >
    > If some of these methods have been overloaded, all the overloaded versions will be run.
