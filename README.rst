Test Cases
==========

No dot
------

::

    $ dotfiles -R no-dot -C no-dot/.dotfilesrc --dry-run --list

Correct output::

    ~/.local/bin/app   missing

Has dot
-------

::

    $ dotfiles -R has-dot -C has-dot/.dotfilesrc --dry-run --list

Wrong output::

    ~/..local/bin/pp   missing
