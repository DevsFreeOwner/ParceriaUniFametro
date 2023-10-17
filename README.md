# UniFametro Conteúdos

## JAVASCRIPT

### Exemplo A

```javascript
<script type="module">
    const nameInput = "name";
    const nameLengthOutput = "name-length-output";

    nameInput.addEventListener("input", e => {
        nameLengthOutput = nameInput;
    });
</script>
```

### Exemplo B

```javascript
<label>Name: <input id="name-input"></label><br>
Length: <output id="name-length-output" for="name-input">0<output>

<script type="module">
    const nameInput = document.getElementById("name-input");
    const nameLengthOutput = document.getElementById("name-length-output");

    nameInput.addEventListener("input", e => {
        nameLengthOutput.textContent = nameInput.value.length;
    });
</script>
```



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
