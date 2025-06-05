# HP-Prime-IEEE754-converter
command line based program that lets the user convert real numbers to IEEE754 binary and vice versa, supports 16,32,64 and 128 bit floats

usage:

toIEEE754(realNumber), you will be prompted to choose either 16, 32, 64 or 128 bit output, it will return a string of bits
ex.

toIEEE754(-2.137)

user chooses 64

"1100000000000001000110001001001101110100101111000110101001111111"



fromIEEE754(stringOfBits), you will be prompted to choose either 16, 32, 64 or 128 bit input, it will return a real number
ex.

fromIEEE754("1100000000000001000110001001001101110100101111000110101001111111")

user chooses 64

−2.137



NOTE:
Te sting of bits that's being provided is rather useless without getting rid of the quotation marks so the easiest way of getting rid of them is by using built-in EXPR() function
ex.
EXPR("#0100000001000110:16b")
will return
#0100000001000110:16b
which is a 16-bit integer that can be nonverted using built-in BASE menu or external functions
