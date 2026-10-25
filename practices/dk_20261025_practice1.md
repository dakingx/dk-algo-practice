# Question
An agent sends a secret message to head quarters containing the details of hisproject. He sends one soft copy to the agency's computer (P) and sends one hard copy by fax to Roger, the technical head of the agency (Q). But during the transmission, noise in the network causes some bits of the data message P to get distorted. However, we know that Roger always matches the binary values of both messages and checks whether he can convert the message P to message Q by flipping the minimum number of bits.

Write an algorithm to help Roger find the minimum number of bits that must be flipped to convert message P to message Q.

# Input
The first line of the input consists of an integer num1, representing the secret message sent to the agency's computer(P)
The second line consists of an integer num2, representing the message sent to the technical head of the agency(Q).

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
