# Dictionary Constants
Writing `String`'s was never that easy.


### Usage
``` java
package de.jmattheis.example;

import de.jmattheis.dictionary.Dictionary;

public class ExampleApplication {
    public static void main(String[] args) {
        System.out.println(Dictionary.hurray);
        // outputs: hurray
    }
}
```

### Words source

The words are taken from [RIDYHEW (RIDiculouslY Huge English Wordlist)](http://www.codehappy.net/wordlist.htm).

### Architecture
The JVM has a limit on constants in a class because of that, the dictionary is splitted in several classes *(30000 constants each)* which inherit each other. The class names of them start with `XDictionary` and are followed by a number.