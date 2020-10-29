# No Jenkins Style Guide

No Jenkins programs use whatever niche shell you run on your machine,
e.g. `fish` or [kitty](https://sw.kovidgoyal.net/kitty/).

We only ask that you not be a monster and wrap your lines at 80 characters.

## Linters

If it worked when you tried it, there's not much else to do.

That said, always validate your crontab, _no one_ gets them right,
even on the tenth try.

The No Jenkins community likes [crontab.guru](https://crontab.guru)
Note: They are not a paid sponsor, but we did receive the product free.

## Logging

Append `&> /dev/null` to all commands and you're good. This will save you
loads of cash on disk space and monitoring.
