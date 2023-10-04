# Regular Expressions

Regular Expressions are text patterns that are used by tools like grep and others&#x20;

* Don't confuse regular expressions with globbing!&#x20;
* They look like file globbing, but they are not the same&#x20;
  * **grep 'a\*' a\***
* For use with specific tools only (**grep, vim, awk, sed**)&#x20;
* See **man 7 regex** for details
* Regular expressions are built around **atoms**; an atom specified what text is to be matched&#x20;
  * Atoms can be single characters, a range of characters, or dot if you don't know the character&#x20;
  * Or atoms can be a class, such as \[\[:alpha:]], \[\[:upper:]] \[\[:allnum:]]
* The second element is the **repetition operator,** which specifies how many times a character should occur
* The third element is indicating where to find the next character.

## Some regular expressions

<table data-full-width="false"><thead><tr><th>Starting characters</th><th align="right">Repetition operators</th></tr></thead><tbody><tr><td><strong>^ :</strong> beginning of the line</td><td align="right"><strong>{n} :</strong> exact n times</td></tr><tr><td><strong>$</strong> : end of the line</td><td align="right"><strong>{n,} :</strong> minimal times</td></tr><tr><td><strong>\&#x3C;</strong> : beginning of a word</td><td align="right"><strong>{,n} :</strong> n times max</td></tr><tr><td><strong>\></strong> : end of a word</td><td align="right"><strong>{n,o}</strong> betwen n and o times</td></tr><tr><td><strong>\A</strong> : start of a file</td><td align="right"><strong>*:</strong> zero or more times</td></tr><tr><td><strong>\Z</strong> : end of a file</td><td align="right"><strong>+ :</strong> one or more times</td></tr><tr><td></td><td align="right"><strong>? :</strong> zero or more time</td></tr></tbody></table>
