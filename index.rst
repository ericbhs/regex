=====================================
Welcome to Regex's tips & tricks!
=====================================

.. contents:: :local:

https://www.youtube.com/watch?v=rhzKDrUiJVk

To test regex: https://regexr.com/

=================== =============================================
Regex				Use
=================== =============================================
``x+``				select at least one occurence of ``x``
``xy?``				``x`` is mandatory, ``y`` is optional
``*``				combination of ``?`` and ``+``, optional but match as many as possible in a row
``.``				match anything but a new line (``'\n'``. To match ``'.'`` escape it with ``\.``
``\w``				match any word (between white spaces ``' '``)
``\W``				match everything that's NOT a word (for example ``' '``, ``'.'``, ...)
``\s``				match white space ``' '`` character
``\S``				match everything that's NOT a white space ``' '`` character
``\d``				any form of number digits
``\d{9}``			any group of 9 number digits in a row
``[xy]z``			match any of these inside the brackets (``'y'`` or ``'y'`` followed by ``'z'``)
``[a-z]``			match anything between ``'a'`` and ``'z'`` character
``()``				create an indepedant group that acts upon itself
``|``				boolean OR
``(t|e|r){2,3}``	match between 2 and 3 of ``'t'`` or ``'e'`` or ``'r'``
``^``				match the beginning of the line
``?``				Lazy, makes the preceding quantifier lazy, causing it to match as few characters as possible
``xyz.+?a``			match any group of characters between ``'xyz'`` and ``'a'``
``$``				match end of statement (activate multiline for every line end)
``(?<=[Tt]he).``	"positive lookbehind", match any character which follows the word "The" (capitalized or not, without selecting the word "the" itself)
``(?<![Tt]he).``	"negative lookbehind", match any character which DOES NOT follow the word "The" (capitalized or not)
``(?=[Tt]he).``		"positive ahead", match any character that is followed by the word "The" (capitalized or not, without selecting the word "the" itself)
``(?![Tt]he).``		"negative ahead", match any character that is NOT followed by the word "The" (capitalized or not)
=================== =============================================