# Question
An agent sends a secret message toheadquarters containing the details of hisproject. He sends one soft copy to theagency's computer (P) and sends onehard copy by fax to Roger, the technicahead of the agency (Q). But during thetransmission, noise in the network causessome bits of the data message P to getdistorted. However, we know that Rogeralways matches the binary values of bothmessages and checks whether he canconvert the message P to message Q byflipping the minimum number of bits.

Write an algorithm to help Roger find theminimum number of bits that must beflipped to convert message P to message Q.

# Input
The first line of the input consists of aninteger num1, representing the secretmessage sent to the agency's computer(P)
The second line consists of aninteger num2, representing the messagesent to the technical head of the agency(Q).

# Output
Print an integer representing the minimum number of bits that must be flipped to convert message P to message Q.

# Constraints
-10^4 <= num1, num2 <= 10^9

# Example
Input:
7
10

Output:
3

Explanation:
Binary representation of P is 00000111.
Binary representation of Q is 00001010.
Three bits of P at position 5, 6 and 8 must be flipped.
So the number of bits that must beflipped is 3.
