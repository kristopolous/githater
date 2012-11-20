githater
========

githater core.

## Don't memorize stupidly named shit.

This system uses some naive linguistic parser that assigns weights to stuff you type after the command line. Then it searches through a database of
useful git things and presents you with explanations.  You know, like a command-line git google.

## Example

    $ githater clone shit more quickly

    Only clone what's necessary to get going instead of everything

      git clone --depth=1

    $ githater create repo without fucked up permissions

    Create a new repository and set the permissions right.

      (  r=<repo-name>.git g=<group-name>;  \
            mkdir $r     \
         && chgrp $g $r  \
         && chmod g+s $r \
         && git init --shared --bare $r \
      )
