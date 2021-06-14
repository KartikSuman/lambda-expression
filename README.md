# lambda-expression are a very powerful tool in projects development as well as in Competitive programming.
They were introduced in c++11 , before which function pointers were used.
As for using a function pointers, we need to create a seperate function , create a pointer to that expression and then pass as a parameter to that required function.
As this is a very cumbersome process, hence lambda expressions came to the scene.

here is an illustration of the difference that we can find in the complexity while implementing a function ponter and while implementing a lambada expression i.e.,a annonymous function.

For sorting the element in descending order,when we use the STl sort function then,

In case of function pointers:--

int descending(int x ,int y)
return x>y;
.
.
.
vector<int>vect{4,2,7,8,0};
sort(vect.begin(),vect.end(),descending);
 . 
 .
 .
 .
  
In case of lambda expression:--

 sort(vect.begin(),vect.end(),[](int x,int y){return x>y;}); 
 
  
