# accumulate

**Description :** This function is used to perform certain operations on the range of iterators provided. It takes two iterators and initial value as parameters.The function is overloaded with first type accepting only these three arguments and returning sum of all elements that can be iterated using the given iterators while the second type takes a binary operation function as additional parameter and performs certain user defined operations on pair of elements pointed by the iterators.


**Example** :

```cpp
int GCD(int x, int y){
	return std::__gcd(x,y);
}

int main() { 

	std::vector<int> v{10, 2, 4, 6}; 
	
	std::cout<<"The sum of elements of v is : "<<accumulate(v.begin(), v.end(),0)<<" and GCD of all elements is : "<<accumulate(v.begin(), v.end(),0,GCD)<<std::endl;
}
```
**[Run Code](https://ideone.com/Gf2d0G)**
