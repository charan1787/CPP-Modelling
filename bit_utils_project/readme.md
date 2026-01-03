

Objective : To learn how numbers are stored and manipulated at the bit level and to write C++ code that behaves exactly the same on every machine.

Implemented Functions : 

  get bits : Extracts a range of bits from a 32-bit unsigned integer.

  set bits : Replaces a range of bits in a 32-bit unsigned integer.

  rotr32 & rotl32 : Performs bit rotation (not the shifting operation).

  sign_extend : Interprets an N-bit value as signed and extends it to 32 bits.


How to run : 
Requirements : 
  C++17 or newer
  g++ or clang++
  
Compile : Linux / mac OS Command : g++ -std=c++17 -Wall -Wextra -O2 main.cpp bit_utils.cpp -o app
Run : ./app

Test Cases : 

  Bit extraction using get_bits
  Bit replacement using set_bits
  Left and right rotations
  Sign extension for positive and negative values

Edge cases such as:
  0xFFFFFFFF + 1
  Negative sign extension


Key Design Decisions : 
  Fixed-width types (uint32_t, int32_t) are used instead of int
  No reliance on undefined behavior
  All operations are deterministic and reproducible
  Signed overflow is avoided
  Right shifts are performed only on unsigned values

