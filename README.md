KMP Alogrithm using to search string in notepad, word file or etc. The pattern are used to show the search result.

Firstly, creating a array for compared string. The array is used to found postition which reback and continues comparing sussessive character in string.
For examples, there is a string "ABCABY" which want to search for matching in other string.
The array which describles postition for this string is belows:
pos   : | 0 | 1 | 2 | 3 | 4 | 5 |
string: | A | B | C | A | B | Y |
algo  : | 0 | 0 | 0 | 1 | 2 | 0 |

Pos2 "C" is not matched, this means pos0 and pos1 is matched. Checking a created array for finding reback postition to start searching.
When pos5 is matched, this string exsisted in the string which found in it.

Check pattern "ABCABY" have existed a text "ABCABCABY" or not.
 text    :ABCABCABY
 pattern :ABCABY
         :     ^

When checking text5"C" is not matched pattern5"Y", this means "ABCAB" is matched each other. pattern4"B" in KMPalgo is 2, string[2] is charater "C".
pattern2"C" is matched text5"C" and continues to search successvice "ABY". All character in pattern is matched, "existed" should return.

For using KMP alogrithm for searching string, O(m+n) time to search instead of O(mn) time.

