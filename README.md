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


## filehandling

* Problem A

	A.in
	```txt
	Hello World
	```
	A.cpp
	```cpp
	#include <iostream>
	#include <cstdio>
	#include <string>
	using namespace std;
	int main(){
		freopen("A.in", "r", stdin);
		string s;
		while(cin >> s){
			cout<< s << endl;
		}
		return 0;
	}
	```
* Problem B

	B.in
	```txt
	Hello
	World
	Clyde
	xxx
	Hi
	```
	B.cpp
	```cpp
	#include <iostream>
	#include <cstdio>
	#include <string>
	using namespace std;
	int main(){
		freopen("B.in", "r", stdin);
		string s;
		while(cin >> s){
			if(s.compare("xxx") == 0)break;
			cout<< s << endl;
		}
		return 0;
	}
	//http://www.cplusplus.com/reference/string/string/compare/
	```
* Problem C

	C.in
	```txt
	3
	Hello
	World
	Clyde
	Hi
	```
	C.cpp
	```cpp
	#include <iostream>
	#include <cstdio>
	#include <string>
	using namespace std;
	int main(){
		freopen("C.in", "r", stdin);
		string s;
		int t;	
		cin >> t;
		while(t > 0){
			cin >> s;
			cout<< s << endl;
			t--;
		}
		return 0;
	}
	```	
