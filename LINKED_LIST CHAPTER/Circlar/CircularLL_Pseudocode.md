# Circular Linked List


## New Node at the Beginning

`IF AVAIL == NULL`
`-->EXIT`
`SET NEW_NODE = AVAIL`
`SET AVAIL = AVAIL->NEXT`
`SET NEWNODE->DATA = VAL`
`SET PTR = START`
`WHILE PTR->NEXT != START`
`-->PTR = PTR->NEXT`
`[END OF LOOP]`
`SET NEWNODE->NEXT = START`
`SET PTR->NEXT = NEWNODE`
`SET START = NEWNODE`
`EXIT`


## Insert New Node at the End

`IF AVAUL == NULL`
`-->EXIT`
`SET NEWNODE = AVAIL`
`SET NEWNODE->DATA = VAL`
`NEWNODE->NEXT = START`
`SET PTR = START`
`WHILE PTR->NEXT != START`
`-->SET PTR = PTR->NEXT`
`[END OF THE LOOP]`
`SET PTR->NEXT = NEWNODE`
`EXIT`


## Delete the First Node

`IF START == NULL`
`-->EXIT`
`SET PTR = START`
`WHILE PTR->NEXT != START`
`-->SET PTR = PTR->NEXT`
`[END OF THE LOOP]`
`SET PTR->NEXT = START->NEXT`
`FREE START`
`SET START = PTR->NEXT`
`EXIT`


## Delete the Last Node

`IF START == NULL`
`--> EXIT`
`SET PTR = START`
`WHILE PTR->NEXT != START`
`-->SET PREPTR = PTR`
`--> SET PTR = PTR->NEXT`
`[END OF THE LOOP]`
`SET PREPTR->NEXT = START`
`FREE PTR`
`EXIT`