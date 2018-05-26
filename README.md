# CMinusCompiler
lexical analyzer and the parser for the c- language
# Installation instructions
1. download javcc from https://javacc.org/download
2. extract archive to the location c:\
3. confirm the availability of C:\javacc-6.0\bin\lib\javacc.jar
4. to generate lexical analyzer, parser and supporting scripts:
```sh
java -cp C:\javacc-6.0\bin\lib\javacc.jar javacc exparser.jj 
```
5. to compile scripts:
```sh
javac *.java
```

6. to parse c- language script: 
```sh
java CMParser input.txt 
```
# Example program of c- language
```sh
/* A program to perform Euclid's
Algorithm to compute gcd.*/
int i;
int gcd (int u, int v)
{
if(v==0) return u ;
else return gcd(v, u-u/v*v);
/* u-u/v*v == u mod v*/
}
void main(void)
{
int x; int y;
x = input(); y = input();
output(gcd(x, y));
}
```

