# fpga
Encryption algorithms for database and FPGA communication channels
# The main algorithm is AES
AES (Advanced Encryption Standard) is a symmetric encryption algorithm that is used to protect data from unauthorized access. AES is widely used in various applications, including Internet security, data storage security, cloud computing, and many other areas.
Main functions:
SubBytes: For each byte in a 16-byte block, replaces its value with the corresponding value from the S-Box, which is a substitution table.

ShiftRows: For each row in a 16-byte block, shifts the bytes by a fixed shift. For example, the first row is left untouched, the second row is shifted 1 byte to the left, the third row is shifted 2 bytes to the left, and so on.

MixColumns: For each column in a 16-byte block, applies a linear transformation that mixes the values in the column. This conversion is performed on bytes represented as elements of the Galois field GF(2^8).

AddRoundKey: Each byte in the 16-byte block is bitwise XORed with the corresponding byte from the round key. The key for each round is generated from the main encryption key using the KeySchedule algorithm.
