# BitArray

A minimal C++ array of bits with clean interface.

#### An example:
```c++
#include "BitArray.h"
#include <iostream>
using namespace std;

int main ()
{
  // Just declare how many bits
  // you want in the array
  BitArray odds (20);

  // Use it exactly like an array!
  for (int i = 0; i < 20; ++i)
    odds [i] = (i % 2 == 1);    // Setting

  for (int i = 0; i < 20; ++i)
    if (odds [i])               // getting
      cout << i << " is odd." << endl;
    else
      cout << i << " is even." << endl;

  return 0;
}
```
