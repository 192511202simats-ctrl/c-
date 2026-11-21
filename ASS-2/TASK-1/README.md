Q1 – Call by Value, by Reference and by Pointer
```
#include &lt;iostream&gt;
using namespace std;
void byValue(long long fee, int percent)
{
fee -= fee * percent / 100;
}
void byReference(long long&amp; fee, int percent)
{
fee -= fee * percent / 100;
}
void byPointer(long long* fee, int percent)
{
*fee -= *fee * percent / 100;
}
int main()
{
long long a = 45000, b = 45000, c = 45000;
byValue(a, 10);
byReference(b, 15);
byPointer(&amp;c, 25);
cout &lt;&lt; &quot;Call by value: &quot; &lt;&lt; a &lt;&lt; &#39;\n&#39;;
cout &lt;&lt; &quot;Call by reference: &quot; &lt;&lt; b &lt;&lt; &#39;\n&#39;;
cout &lt;&lt; &quot;Call by pointer: &quot; &lt;&lt; c &lt;&lt; &#39;\n&#39;;
return 0;
}
```
