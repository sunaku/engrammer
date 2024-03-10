[Arno's Engram]: https://engram.dev

# Engrammer - [Arno's Engram] layout for programmers

This is a programmer-friendly variant of [Arno's Engram] 2.0 keyboard
layout that helps maintain cross-proficiency with standard keyboards:

* Shifted pairs are standard (e.g. quotes don't shift to parentheses).
* Semicolon is placed relative to comma and period just like standard.
* Equals and square brackets are placed near their standard locations.

In addition, application shortcuts that assume standard shifted pairs,
such as Control-Equals for the "zoom in" operation, now work properly.

To illustrate the differences between this layout, Engram, and QWERTY:

>*Legend:* Gold is [Arno's Engram]; Blue is Engram-like; Pink is new.
>![Rendering of this layout on a standard 60% keyboard.](https://raw.githubusercontent.com/sunaku/engrammer/main/layout.png)
>![Rendering of this layout on an ortholinear keyboard.](https://raw.githubusercontent.com/sunaku/engrammer/main/ortho.png)
>
>     `~ 1! 2@ 3# 4$  5%  6^  7& 8* 9( 0) [{ ]}
>        bB yY oO uU  '"  ;:  lL dD wW vV zZ =+ \|
>        cC iI eE aA  ,<  .>  hH tT sS nN qQ
>        gG xX jJ kK  -_  /?  rR mM fF pP

For example, here are my split ortholinear keyboards using this layout:

* This is [my Glove80](https://sunaku.github.io/moergo-glove80-keyboard.html) keyboard by MoErgo:
>![Photo of MoErgo Glove80](https://raw.githubusercontent.com/sunaku/sunaku.github.io/master/moergo-glove80-keyboard-photograph.jpg)
>![Layout of MoErgo Glove80](https://raw.githubusercontent.com/sunaku/sunaku.github.io/master/moergo-glove80-keyboard-base-layer.png)

* This is [my Remnant](https://sunaku.github.io/ergohaven-remnant-keyboard.html) keyboard by Ergohaven:
>![Photo of Ergohaven Remnant](https://raw.githubusercontent.com/sunaku/sunaku.github.io/master/ergohaven-remnant-keyboard-photograph.jpg)
>![Layout of Ergohaven Remnant](https://raw.githubusercontent.com/sunaku/sunaku.github.io/master/ergohaven-remnant-keyboard-base-layer.png)

## Linux setup

Install:

    cd linux/
    sudo make install
    echo Now restart your graphical session.

Activate:

    setxkbmap -layout us    -variant engrammer         # one layout; no switch
    setxkbmap -layout us,us -variant engrammer,basic   # dual layout switching

Repair (e.g. whenever a system-wide XKB package upgrade reverts installation):

    cd linux/
    sudo make reinstall
    echo Now restart your graphical session.

Uninstall:

    cd linux/
    sudo make uninstall
    echo Now restart your graphical session.

## Windows setup

You can [download a pre-built installation package](
  https://github.com/sunaku/engrammer/releases/download/windows/engrammer.zip
) or build one yourself, like this:

1. Install the official _Microsoft Keyboard Layout Creator_ app: [MSKLC version 1.4](
  https://www.microsoft.com/en-us/download/details.aspx?id=102134
).

2. Launch the MSKLC app and open up the `windows\engrammer.klc` source file.

3. From the "Project" menu, select the "Build DLL and Setup Package" action.

4. Open the resulting build directory and run the `setup.exe` installer file.

## MacOS setup

1. Copy `macos/Engrammer.bundle` to `~/Library/Keyboard Layouts/` directory

2. Log out and Log in again to your MacOS user

3. Open Keyboard Settings and add Engrammer from the list of English layouts

## Type Fu setup

![type-fu.com](https://github.com/sunaku/engrammer/assets/9863/f90439c8-3d96-4902-b471-45511fba8c33)

1. Launch the [Type Fu](https://type-fu.com/) app, then open the "More" menu.

2. Go to Preferences > Keyboard > Functional > "More" menu > Import from file.

3. Pick the `type-fu.com/engrammer.tfl` file from your copy of this repository.

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
