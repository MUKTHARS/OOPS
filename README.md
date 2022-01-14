class test
{
int x;
public:
static void fun()
{
cout<<x;
}
};

OUTPUT : Error        Trying to access member function than instance function


class test
{
static int x;//declaration
public:
void fun()
{
cout<<x;
}
};
int test:: x=0 ; // declaration


class test                                  1 . x and fun are static --> correct
{int x;                                     2.x-> instance , fun-> static   -----> wrong
public:                                     3.x and fun are instance ----> correct
void fun()                                  4. x-> static ,fun ->instance  ------> correct
{
const<<x;
}
};

we can also make constructor as private
