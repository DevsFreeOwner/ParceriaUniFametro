# UniFametro Conteúdos


## JAVA

### Exemplo A

```java
//Main Método
public static void main(String args[]){

      var variavel = "globalVariable"
      System.out.println("globalVariable:" + variavel);

      variavel = "newglobalValue";
      System.out.println("globalVariable:"+ variavel);

}
```

### Exemplo B

```java
//Global Class
public class GlobalClass {
            public static String globalVariable = "globalValue";
}

//Main Método
public static void main(String args[]){

      System.out.println("globalVariable:"+GlobalClass.globalVariable);
      GlobalClass.globalVariable = "newglobalValue";
      System.out.println("globalVariable:"+GlobalClass.globalVariable);

}
```
