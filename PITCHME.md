# Unit testing is easy ...

+++

## ... but I am QA. Why should I care?

---

#What good test is? 

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

##Validates design and implementation

+++

##Testing of pure logic 

---

#Structure, Naming ... 

+++

##Java Project 

+++

###Production and Test contexts
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

##@RunWith

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
        // give
        Gitar gitar = new Gitar();
        // when
        String actualSound = gitar.play();
        // then
        assertEquals(Gitar.BRUNNNN, actualSound);
    }

}
```

---?image=assets/rockgroup.jpg&size=auto 100%

+++

##Let's rock!

+++

##Coverage: class, line, branch

---

##Unit tests are not always easy

+++

##Static methods

+++

##Monster classes
![monsterClass](assets/monster.jpg)

+++

##Refactoring may become a trap

---

#Summary

+++

##Life is hard without unit tests

+++

##Untestable code mean bad design

+++

##Developer does unit testing

+++?image=assets/questions.png&size=auto 100%
