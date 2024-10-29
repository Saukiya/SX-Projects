import Tabs from '@theme/Tabs'
import TabItem from '@theme/TabItem'

<Tabs>
  <TabItem value="apple" label="Java" default>
```java
public class TestCommand extend SubCommand {

    public void test() {
        System.out.println("HelloWorld!");
    }

}

```
  </TabItem>
  <TabItem value="orange" label="Kotlin">
```kotlin
class TestCommand : SubCommand() {
    fun test() {
        println("Hello, World!")
    }
}
```

  </TabItem>
</Tabs>