KnightMove
==========

C++ Solution


Task:
To find all 10-key sequences that can be keyed into the keypad in the following manner:
- The initial keypress can be any of the keys from keypad.
- Each subsequent keypress must be a knight move (aka chess) from the previous keypress.  
- There can be at most 2 vowels in the sequence.

A knight move is made in one of the following ways:
- two steps horizontally and one step vertically.
- two steps vertically and one step horizontally.

Keypad:

A B C D E 

F G H I J

K L M N O

'. 1 2 3. '
  

Solution notes:
1) do table of possible transitions:
A-HL
B-IKM
C-FJLN
D-GMO
E-HN
F-CM
G-DN2
H-AEKO13
I-BL2
J-CM3
K-BH2
L-ACI3
M-BDFJ
N-CEG1
O-DH2
1-FHN
2-GIKO
3-HL

2) Used recursive search.
KnightMove cpp 