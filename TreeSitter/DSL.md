**rule**

| F                   | arg                         | ?                                           |
| ------------------- | --------------------------- | ------------------------------------------- |
| **seq**             | _list\<rule\>_              | конкатенация правил                         |
| **choice**          | *list<rule\>*               | regExp **\|**                               |
| **repeat**          | *rule*                      | regExp __\*__                               |
| **reepeat1**        | *rule*                      | regExp **+**                                |
| **token**           | *rule*                      | regExp as only 1 token                      |
| **token.immediate** | *rule*                      | token if !*extra*( комментарий или пробел ) |
| **alias**           | *rule*, *name: str \| rule* | alt имя=**name** для **rule**               |
| **field**           | *name: str*, *rule*         |                                             |
