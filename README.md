# cppnotes

* Install [Codeblocks](http://www.codeblocks.org/downloads) (binary realease)
* Navigate to Program Files (x86) > Codeblocks > MinGW > bin and copy the directory path
* Edit Windows Environment Variables then paste the path
* Open command prompt and verify g++ version installed using ```$ g++ --version```
* Write cpp code
```cpp
#include <iostream>
using namespace std;
int main(){
	cout<<"Hello World";
	return 0;
}
```
* Compile using ```$ g++ -o A A.cpp```
* Execute using ```$ A```
