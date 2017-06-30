# Unit testing is easy ...

+++

# ... but I am QA. Why should I care?

---

#What good test is? 

+++

#Strong

+++ 

#Maintainable

+++

#Readable

+++

#Fast

---

#Why testing in isolation?

---

#Structure, Naming ... 

+++

#Java Project: main and test

+++

#@RunWith

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



