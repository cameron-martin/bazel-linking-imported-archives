```
g++ -c bar.cpp -o bar.o
ar -rcs bar.a bar.o
bazel test //:test
```