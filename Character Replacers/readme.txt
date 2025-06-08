Character Replacers (CR);

Character replacers are libraries that work on automatic trigger (*) syntax.
They serve different purposes depending on language.
For example, for Indic scripts, they can serve to replace maatras with independent vowels at the start of words.
This automates something that is supposed to be automated but isn't done by the computer while typing.

In Latin alphabet scripts such as Vietnamese, the composite character replacer replaces multiple Unicode characters with single characters.
For example, the user types (ê), latin small letter e with circumflex (U+00EA), then types combining acute accent (U+0301).
The program automatically replaces what was typed with (ế), latin small letter e with circumflex and acute (U+1EBF).
This causes a decrease in filesize by one byte.
Otherwise, the composite character replacement is not a necessary operation.


Maatra Helpers — Help Documentation;

I created these Hotstrings.exe libraries to tackle an issue concerning typing vowels in Indic scripts.

In the Devanagari alphabet, vowels can be written in two ways, the independent vowel forms and the maatra forms.
(https://en.wiktionary.org/wiki/matra)

This creates a challenge when typing Indic scripts because we have to make four separate key assignments for vowels.
Maatra, vowel, long maatra, long vowel.

In the computer programs I created to type Indic scripts, the vowel keys give us the maatra forms while pressing CapsLock+Vowel keys gives us the independent vowel forms.
Pressing Shift+Vowel keys gives us long maatra forms and pressing CapsLock+Shift+Vowel keys give us independent long vowel forms.

This seemed like a good idea because Indic scripts are caseless.
So I figured out a method for using the CapsLock key as an extra modifier key.

I created this computer program to facilitate this matter:
https://github.com/SalviaSage/Autohotkey-Scripts-Repository/tree/master/Typing%20Scripts/Holdable%20CapsLock

This program makes the caps lock key behave just like the shift key, but it does not make it a Shift key.
This is good because we still need the shift key as a separate modifier key.

However, this makes it so that the maatras are typed at the start of words where the independent vowel forms would be.
For example, the typist would want to type उत्तर (uttar) but would get ुत्तार instead.

This mistake would never be made if writing with a pen and paper.

In this scenario, this is done intentionally since the maatra and the independent vowels are treated as different letters by the computer.
The computer does not automate the maatra placements but I got the idea to see if it could be automated and succeeded in finding a way.
It could not be a reality until I found out about the computer program Hotstrings.exe.

The typist would have to press separate keys or press Shift+Key to type independent vowel letters.
That itself is good in the sense that it gives us a manual way of typing whichever maatra or vowel letter we want to type.
However, it introduces the problem where the maatra is used where it cannot be used.
Most typically, the first letter of a word.

So, what these custom libraries do is that they automatically detect and delete the starting maatras and replace them with their independent vowel forms.

It is an indispensable program for typing with Devanagari and other Indic scripts.

This custom library is based on the program found here:
https://github.com/mslonik/Hotstrings
I am not the author of this program and that program is in active development.
