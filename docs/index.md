# Developer Home


This is the developer home for Paycorp. We will show you how to integrate to paycorp.io


``` js linenums="1" hl_lines="2"
document$.subscribe(function() { //
  var tables = document.querySelectorAll(/*  */ "article table")
  tables.forEach(function(table) {
    new Tablesort(table)
  })
})
```


=== "C"

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```
