Query terminal
=================

.. only:: man

    Overview
    --------------


This kitten is used to query |kitty| from terminal programs about version, values
of various runtime options controlling its features, etc.

The querying is done using the (*semi*) standard XTGETTCAP escape sequence
pioneered by xterm, so it works over SSH as well. The downside is that it is
slow, since it requires a roundtrip to the terminal emulator and back.

If you want to do some of the same querying in your terminal program without
depending on the kitten, you can do so, by processing the same escape codes.
Search `this page <https://invisible-island.net/xterm/ctlseqs/ctlseqs.html>`__
for *XTGETTCAP* to see the syntax for the escape code. The kitty specific keys
are all documented below, when sent via escape code they must be prefixed with
``kitty-query-``.


.. include:: ../generated/cli-kitten-query_terminal.rst
