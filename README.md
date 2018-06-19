# MTF
Move to Front
MTF (move-to-front) algorithm is a data encoding method used to improve the data compression technology. The main use of the data is "spatial locality", that means the characters that have recently appeared are likely to appear again near the next text.
MTF's main idea is:
(1) maintains a stack of text character sets, "recently used symbols", each of the different characters occupies a position in it, starting with a number from 0.
(2) Scan the text data that needs to be re-encoded. For each scanned character, use the character to replace the index in "recently used symbols" and refer the character to the top of the "recently used symbols", index is at position of 0.
(3) Go to (2) until the text scan ends.
In this program, you can input any characters within "abcdefghijklmnop", it output the index of the symbol in the symbol table, then move that symbol to the front of the symbol table "abcdefghijklmnop". In the class MTF, the user can access elements by their integer index (position in the list), and search for elements in the list. Then use the principal operations on a StringBuilder, which are overloaded so as to accept data of any type. Each effectively converts a given datum to a string and then appends or inserts the characters of that string to the string builder. Then converts this string to a new character array.
