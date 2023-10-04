---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: false
  outline:
    visible: false
  pagination:
    visible: true
---

# Finding which man Page to use

_**`man -k user`**_` ``: search the word user and all commands related to it`

_**`man -k | wc`**_ `: aka word count shows how many lines, words and characters this word appeared`

_**`man -k | grep 8 | grep create`**_` ``: sends the result of the first command to the next so that it filters in section 8 and to the word create`

_**`man -k carmel`**_` ``: is going to show nothing inapropriate it can happen also wwhen you type man -k user`

_**`mandb`**_` ``: will update the man database type it when you get nothing inapropriate`
