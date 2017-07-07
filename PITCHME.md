##Tests
#will safe
##the world
---
# Unit testing is easy ...
+++
## ... but I am QA ...
##Why should I care?
---
##What is a
#good test? 
+++
##Strong
+++
##Maintainable
+++
##Readable
+++
##Fast
---
#Why testing in isolation?
+++
##Validates design
+++
##Pushes towards refactoring
+++
##Checks only logic
+++
##Identifies dependencies
---
#Java Project 
+++
###Naming
```
main/
  java
    com.company
      MyClass
test/
  java
    com.company
      MyClassTest
```
+++
###Production and Test
###contexts
---
#JUnit
+++
##@Test
+++
##@RunWith
+++
##Each test
##runs
##in separate thread
+++
##Test structure
+++
```
public class Gitar {

    static final String BRUNNNN = "Brunnnn..";

    public String play() {
        return BRUNNNN;
    }
}
```
```
public class GitarTest {

    @Test
    public void play() throws Exception {
        // given
        Gitar gitar = new Gitar();
        // when
        String actualSound = gitar.play();
        // then
        assertEquals(Gitar.BRUNNNN, actualSound);
    }

}
```
---
#Let's rock!
+++?image=assets/rockgroup.jpg&size=auto 100%
##Coverage: class, line, branch
---?image=assets/monster.jpg&size=auto 50%
+++
##Monster methods/classes
+++
##Static dependencies
+++
##Refactoring may become a trap
---
#Summary
+++
##Life's hard
###without
##unit tests
+++
##Tests
###should not
##depend on implementation
+++
##Untestable code
###means
##bad design
+++
##Developer
###does do
##unit testing
+++
##Quality engineer 
###does NOT do
##unit testing 
---?image=assets/questions.png&size=auto 50%