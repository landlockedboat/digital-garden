* It is actually better to make variable assignmets using the list notation 
`double d {2.2}` as it protects us from conversions that lose information such 
as `int i = 7.2 // i is now 7`. The = operator for assignment is actually 
outdated and mantained only for C compatibility!

* Range-for-statement
```
for (auto x:v)
  cout << x << endl;
```
More efficient
```
for (auto& x:v)
  cout << x << endl;
```
