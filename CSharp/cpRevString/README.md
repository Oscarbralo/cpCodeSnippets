cpRevString
===========

This is a little code snippet to use when you need to reverse a string.

StringBuilder $newString$ = new StringBuilder();
            for (int i = $yourString$.Length - 1; i >= 0; i--)
            {
                $newString$.Append($yourString$[i]);
            }

The first $newString$ is the name of your StringBuilder variable.
The second one $yourString$ is the name of the string you want to reverse.
