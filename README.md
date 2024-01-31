[Arno's Engram]: https://engram.dev

# Engrammerdvp - [Engrammer] layout for programmers.
This is a programmer-friendly variant of Engrammer which itself is a variant of [Arno's Engram] 2.0 keyboard layout that helps speed up programming by putting the symbols in a better position inspired by the Programmer Dvorak layout. Why a new layout? As nice as it is, engrammer has some serious problems when writing source code. The characters are in an en layout all right, but the symbols are put in the same hopeless locations as in the Qwerty layout!
 
* Semicolon is placed relative to comma and period just like standard.
* This sub-layout makes it easier to write source code in C, C#, Java, Pascal, Lisp, CSS, XML and alikes by incorporating the symbol layout Programmer Dvorak. It was generated through reflection of the most common constructs in these languages and the rules set forward by the August Dvorak in his research, then verified by scanning through thousands of source code lines ensuring that a good fit was found.
* In contrast to engrammer, this layout does not attempt to preserve application shortcuts that assume standard shifted pairs, such as Control-Equals for the "zoom in" operation. It instead focuses solely on increasing speed when typing source. 
To illustrate the differences between this layout, Engrammer, Engram, and QWERTY:

Engrammerdvp
>     $~ &% [7 {5 (3  +1  =9  )0 }2 ]4 *6 !8 #`
>        bB yY oO uU  '"  ;:  lL dD wW vV zZ @^ \|
>        cC iI eE aA  ,<  .>  hH tT sS nN qQ
>        gG xX jJ kK  -_  /?  rR mM fF pP

Engrammer
>     `~ 1! 2@ 3# 4$  5%  6^  7& 8* 9( 0) [{ ]}
>        bB yY oO uU  '"  ;:  lL dD wW vV zZ =+ \|
>        cC iI eE aA  ,<  .>  hH tT sS nN qQ
>        gG xX jJ kK  -_  /?  rR mM fF pP

Engram     
>     [{ 1| 2= 3~ 4+  5<  6>  7^ 8& 9% 0* ]} /\
>        bB yY oO uU  '(  ")  lL dD wW vV zZ #$ @`
>        cC iI eE aA  ,;  .:  hH tT sS nN qQ 
>        gG xX jJ kK  -_  ?!  rR mM fF pP






## Linux setup

Install:

    cd linux/
    sudo make install
    echo Now restart your graphical session.

Activate:

    setxkbmap -layout us    -variant engrammer 

Repair (e.g. whenever a system-wide XKB package upgrade reverts installation):

    cd linux/
    sudo make reinstall
    echo Now restart your graphical session.

Uninstall:

    cd linux/
    sudo make uninstall
    echo Now restart your graphical session.


## License

Released under the same terms as [Arno's Engram]:

> MIT License
>
> Copyright 2021 Arno Klein
>
> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice shall be included in
> all copies or substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.
