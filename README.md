<div align="center">

## Basics of C/C\+\+ Part 5: Switch\.\.\.Case


</div>

### Description

I know that this is probably a let-down, after you learned all about functions, but switch...case is important to know. After all, it can save space with if statements, and it is useful. Besides, I couldn't think of anything else that I wanted to write about!
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Alexander of CProgramming\.com](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/alexander-of-cprogramming-com.md)
**Level**          |Beginner
**User Rating**    |4.0 (12 globes from 3 users)
**Compatibility**  |C, C\+\+ \(general\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__3-1.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/alexander-of-cprogramming-com-basics-of-c-c-part-5-switch-case__3-457/archive/master.zip)





### Source Code

<p> </p>
<p><font face="Verdana">     Switch...case looks like this:</font></p>
<p><font face="Verdana">switch(expression or variable)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">case it equals this:</font></p>
<p><font face="Verdana">do this;</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">case it equals this:</font></p>
<p><font face="Verdana">do this;</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">case it equals this:</font></p>
<p><font face="Verdana">do this;</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">...</font></p>
<p><font face="Verdana">default</font></p>
<p><font face="Verdana">do this</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">     So, it works like this. The
expression or variable has a value. The case says that if it has the value of
whatever is after this case then do whatever follows the colon. The break says
to break out of the case statements. Break is a keyword that breaks out of the
code-block, surrounded by braces, that it is in. So unless you want it to try
the next case then use break. --You can also use it to break out of loops,
something that I failed to mention at the time.--</font></p>
<p><font face="Verdana">     What is it used for, the
switch...case? Well, let's say that you are writing a menu program, then you
would want to process some input, right? Well, you would want to use a
switch...case statement to process more than one input, because it is more
easily used than if statements.</font></p>
<p><font face="Verdana">Here is an example program:</font></p>
<p><font face="Verdana">#include <iostream.h></font></p>
<p><font face="Verdana">#include <conio.h></font></p>
<p> </p>
<p><font face="Verdana">void main()</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">char input;</font></p>
<p> </p>
<p><font face="Verdana">cout<<"1. Play game";</font></p>
<p><font face="Verdana">cout<<"2. Load game";</font></p>
<p><font face="Verdana">cout<<"3. Play multiplayer";</font></p>
<p><font face="Verdana">cout<<"4. Exit";</font></p>
<p><font face="Verdana">input=getch(); //Remember I said you don't need many
functions...</font></p>
<p><font face="Verdana">switch(input)</font></p>
<p><font face="Verdana">{</font></p>
<p><font face="Verdana">case 1:</font></p>
<p><font face="Verdana">playgame();</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">case 2:</font></p>
<p><font face="Verdana">loadgame();</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">case 3: //Note use of : not ;</font></p>
<p><font face="Verdana">playmultiplayer();</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">case 4:</font></p>
<p><font face="Verdana">break;</font></p>
<p><font face="Verdana">default:</font></p>
<p><font face="Verdana">cout<<"Error, bad input, quitting";</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">}</font></p>
<p><font face="Verdana">     If you are not understand this,
then try putting in if statements for the case statements.  Also, the
reason exit works with a break is that after you break out of the switch statement
then it would be the end of the program. The same thing would be for default. 
If you don't like that, then make a loop around the whole thing. I know I did
not  prototype the functions, but it was a very simple example. You could
easily make a few small functions.</font></p>

