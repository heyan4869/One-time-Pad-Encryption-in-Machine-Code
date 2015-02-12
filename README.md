## One-time Pad Encryption in Machine Code

Often we have a message that we want to keep secret from some third party. For example, we want to email someone our social security number, but don’t want anyone who intercepts our email to be able to read it. There are many such encryption schemes, and designing good encryption schemes and secure transmission protocols is a very active area of research. One-time pad is one such encryption scheme that is ancient.

Suppose we have a message t, encoded as stream of bits:

`t = 010101000000011111100010101`

If we have a secret key s of the same length:

`s = 111101010001111100101010101`

We could encrypt t by computing r = t XOR s, where XOR is the function so that sets the ith bit of r based on the ith bits of t and s.
