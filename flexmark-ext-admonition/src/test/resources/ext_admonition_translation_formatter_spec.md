---
title: Admonition Extension Formatter Spec
author: Vladimir Schneider
version: 0.1
date: '2018-03-05'
license: '[CC-BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/)'
...

---

## Admonition Extension

### Basic Tests

```````````````````````````````` example Basic Tests: 1
!!! note
    first child paragraph  
.
!!! note
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


with title

```````````````````````````````` example Basic Tests: 2
!!! note "Title"
    first child paragraph  
.
!!! note "tiItLeE"
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


no heading

```````````````````````````````` example Basic Tests: 3
!!! note ""
    first child paragraph  
.
!!! note ""
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


collapsed

```````````````````````````````` example Basic Tests: 4
??? note
    first child paragraph  
.
??? note
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


collapsed with title

```````````````````````````````` example Basic Tests: 5
??? note "Title"
    first child paragraph  
.
??? note "tiItLeE"
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


collapsed with empty title

```````````````````````````````` example Basic Tests: 6
??? note ""
    first child paragraph  
.
??? note ""
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


open

```````````````````````````````` example Basic Tests: 7
???+ note
    first child paragraph  
.
???+ note
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


open with title

```````````````````````````````` example Basic Tests: 8
???+ note "Title"
    first child paragraph  
.
???+ note "tiItLeE"
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


open with empty title

```````````````````````````````` example Basic Tests: 9
???+ note ""
    first child paragraph  
.
???+ note ""
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


indented 1

```````````````````````````````` example Basic Tests: 10
 ???+ note ""
    first child paragraph  
    
.
???+ note ""
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


indented 2

```````````````````````````````` example Basic Tests: 11
  ???+ note ""
    first child paragraph  
    
.
???+ note ""
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


indented 3

```````````````````````````````` example Basic Tests: 12
   ???+ note ""
    first child paragraph  
    
.
???+ note ""
    FiIRSt chiILD paARaAGRaAph
````````````````````````````````


indented 4

```````````````````````````````` example Basic Tests: 13
    ???+ note ""
        first child paragraph  
    
.
    ???+ note ""
        first child paragraph  
````````````````````````````````


nested

```````````````````````````````` example Basic Tests: 14
???+ note ""
    first child paragraph  
    
    !!! note
        embedded
.
???+ note ""

    FiIRSt chiILD paARaAGRaAph

    !!! note
        eEmBeEDDeED
````````````````````````````````


with multiple children

```````````````````````````````` example Basic Tests: 15
!!! note "Title" 

    ## Heading 2
    
    * bullet list item 1
    * bullet list item 2
    * bullet list item 3
    
    
    | Table Heading  |
    |---|
    | Table Data  |

.
!!! note "tiItLeE"

    ## heEaADiING 2

    * BuULLeEt LiISt iIteEm 1
    * BuULLeEt LiISt iIteEm 2
    * BuULLeEt LiISt iIteEm 3


    | taABLeE heEaADiING  |
    |---|
    | taABLeE daAtaA  |
````````````````````````````````


collapsed with multiple children

```````````````````````````````` example Basic Tests: 16
??? example 

    ## Heading 2
    
    * bullet list item 1
    * bullet list item 2
    * bullet list item 3
    
    
    | Table Heading  |
    |---|
    | Table Data  |

.
??? example

    ## heEaADiING 2

    * BuULLeEt LiISt iIteEm 1
    * BuULLeEt LiISt iIteEm 2
    * BuULLeEt LiISt iIteEm 3


    | taABLeE heEaADiING  |
    |---|
    | taABLeE daAtaA  |
````````````````````````````````


with lazy continuation of first paragraph

```````````````````````````````` example Basic Tests: 17
!!! note
lazy continuation 
.
!!! note
    LaAZyY coNtiINuUaAtiIoN
````````````````````````````````


