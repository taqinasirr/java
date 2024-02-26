JDK
* java development kit
* software development environment for building java app
* has a compiler
* has a bunch of code we can use
* has java runtime environment
* Java SE = java standard edition. (google oracle java se utk download dia) (java SE tu dlm dia ada JDK)
* download code editor - intelliJ idea community edition (free)
* pake vscode pun boleh martt. install extension - 'Extension Pack for Java' so nanti muncullah btn utk run java
* when u install JDK, u get JRE and JVM

commands
* java --version   //show java version
* javac --version  //show java compiler version
* javac Hello.java  //compile Hello.java.  so nanti akan muncul file hasil drpd compile iaitu Hello.class  (ni adalah byte code, yakni language yg JVM faham)
* java Hello   //run file Hello.java   //Hello adalah nama class kat file Hello.java.  dlm class tu ada main()


java is platform independent ( u can run java program on any machine)
* but that machine need to have JVM
* JVM itself is platform dependent. cth, u cant run JVM on ios
* JVM only understand byte code
* Java code --> javac (compiler) --> byte code
* JVM tu yg akan run main() method
* bila run Hello.java, javac akan compile dia jadi bytecode. so, Hello.class akan otomatik muncul. (Hello.class tu adalah byte code)
* JVM is part of JRE
* javac is only for developlemt purpose
* rumusan - dlm JDK ada JRE.  dlm JRE ada JVM

java = strongly typed language

data type
* primitive
   1. int
      * byte   - 1 byte  `byte b = 127;`
      * short  - 2 bytes `short s = 558;` 
      * int    - 4 bytes 
      * long   - 8 bytes `long l = 5854l;`
   3. float  
      * double  - `double num = 1.5;`
      * float   - `float num = 1.5f;`
   5. char
      * 2bytes
      * `char c = 'k';`
   8. boolean
      * true or false shj. x pake 0 utk false 1 utk true
      * `bool b = true;`

<br>

`JDK` `JRE` `JVM` 

![JDK JRE JVM](https://github.com/taqinasirr/java/assets/21170527/24b131f6-3593-4789-bfb9-a327aeaccb2d)

<br>

exception = runtime error = error that happen at runtime. masa compile x dak error

property
* .length
* 

<br>

String          - non modifiable   
StringBuilder   - modifiable.   for string manipulation. cth  reversing a string using reverse(),  inserting a character using insert()    
StringBuffer    - thread safe.   rarely used

<br>

encapsulation
* privatekan  properties. class tu shj boleh access properties tu directly.
* class lain nak access properties tu, kena access melalui method class tu yg return value properties yg privatet tu.

constructor
* method yg nama dia sama nama class
* everytime kita create object, constructor method run tanpa di call.
* if create 2 objek, 2 kali lah constructor method di run
* constructor tu boleh method overloading
  * satu xdak parameter (default constructor)
  * satu ada parameter (parameterized constructor)
* right click, source action, generate constructors

inheritence
* parent -> child   or   super class -> sub class

multi level inheritence  - A super kpd B, B super kpd C.   C inherit methods dari A dan B

multiple inheritence java x support. cth  A super kpd C. B juga super kpd C.  benda ni takdak sebab cth kat A dgn B ada method show() java taktau nak pilih mana satu.

method overriding
* A super kpd B
* A dgn B ada method yg nama dia sama. cth show()
* B obj = new B();
* bila obj.show()  dia akan pakai show() yg kat class B bukan yg kat class A


package
* package = folder
* bubuh classes berkaitan dlm folder (classes tu dlm java file ler)
* cth folder nama haiwan dlm dia ada ayam.java  dgn lembu.java
* java file tu, atas sekali kena letak `package haiwan;`
* main method ada kat luar package. if kat main method nak pakai class dlm ayam.java, kena `import haiwan.ayam'
* `import haiwan.*;` maksudnya import semua java file dlm package haiwan.

polymorphism
* poly = many    morphism = behaviour
* compile time polymorphism - utk method overloading (method nama sama, parameter tak sama, masa compile dah tahu nak pake yg mana satu)
* run time polymorphism - utk method overridding (method parent & child nama sama, parameter sama, masa runtime baru tahu nak pake yg mana satu)
* 
  




