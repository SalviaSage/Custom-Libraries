Input Method Editors (IME)s — Help Documentation; 

These libraries give us IMEs. (Input Method Editors)
They are menus that pop up under the caret which allow us to choose extra letters and characters.
They are necessary for languages and writing systems that have many different letters and diacritics.

The way they work is that they read what was typed with the keyboard and organise a menu based on
what it is that was typed, then we press a certain trigger key to show the menu which is recommended to be the TAB key.

So for example, in Vietnamese IME, we type (a) then we hit the defined trigger character (TAB).
Then we see a menu which lists: 1. á
                                2. à
                                3. ả
                                4. ã
                                5. ạ
Then, we hit the number key on the keyboard;
for example hitting (3) will delete the (a) that we wrote and will type (ả).
We can also select the entry from the list with the mouse.

However, there are some bugs related to spacing and you may see spaces appear before or after the inserted letters.
There is also a bug where we can not enter or type the characters from the keyboard, the mouse selection works better at the moment.

For characters where there is only 1 entry in the menu, the menu should be canceled altogether in favor of automatic conversion upon pressing the tab key.
This can be achieved by changing the 'MSI' syntax to 'SI' syntax in the library file.
