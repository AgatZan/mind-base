**sym** = `$.something`
**rule** = *str | F*

| F                   | arg                        | ?                                           |
| ------------------- | -------------------------- | ------------------------------------------- |
| **seq**             | _list\<rule\>_             | конкатенация правил                         |
| **choice**          | *list<rule\>*              | regExp **\|**                               |
| **repeat**          | *rule*                     | regExp __\*__                               |
| **reepeat1**        | *rule*                     | regExp **+**                                |
| **token**           | *rule*                     | regExp as only 1 token                      |
| **token.immediate** | *rule*                     | token if !*extra*( комментарий или пробел ) |
| **alias**           | *rule*, *name: str \| sym* | alt имя=**name** для **sym**                |
| **field**           | *name: str*, *rule*        | Именовать **rule** именем **name**          |
