cpRevStringSwapping
===================

This is a little code snippet to use when you need to reverse a string swapping the elements.

StringBuilder $newString$ = new StringBuilder($yourString$);
            int j = $yourString$.Length - 1;
            for (int i = 0; i < $yourString$.Length / 2; i++)
            {
                string temp = $newString$[i].ToString();
                $newString$[i] = $newString$[j];
                $newString$.Insert(j, temp);
                $newString$.Remove(j + 1, 1);
                j--;
            }

The first $newString$ is the name of your StringBuilder variable.
The second one $yourString$ is the name of the string you want to reverse.
