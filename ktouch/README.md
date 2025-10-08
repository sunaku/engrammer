This directory contains pre-generated lessons which can be directly imported into ktouch.

1. ktouch-lessons-1.xml and ktouch-lessons-2.xml - Created using [ktgen](https://github.com/BarbieCue/ktgen).
   This can be regenerated running `make ktouch-lessons-2.xml`.
1. ktouch-lessons-2.xml - Created using
   [ktouch-lesson-generator](https://github.com/simgunz/ktouch-lesson-generator) .

[Google Top 10000 English words without swear words](https://raw.githubusercontent.com/first20hours/google-10000-english/refs/heads/master/google-10000-english-usa-no-swears.txt) is used as the dictionary.

For technically inclined, these can be recreated by deleting the lessons and running `make all`.
