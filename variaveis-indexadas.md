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

## Csharp (.net)

### Exemplo A

```csharp
using System;


namespace ErrorTest
{
    class Program
    {
        static void Main(string[] args)
        {
            string a = "Mensagem";
            Console.WriteLime("Sua mensagem foi:" + a);
        }
    }
}
```

### Exemplo B

```csharp
using System;


namespace ErrorTest
{
    class Program
    {
        static void Input(ref string a)
        {
            Console.Write("Por favor insira algo:");
            a = Console.ReadLine();
        }
        static void Output(string a)
        {
            Console.WriteLine("Digite algo: {0}", a);
        }

        static void Main(string[] args)
        {
            string a;
            Input(ref a);
            Output(a);
        }
    }
}
```

## Python

### Exemplo A

```python
class Box:
    width = 100
    height = 200
    weight = 80

print(Box.width) # 100

# Você poderia usar instâncias para atualizar atributos em instâncias separadas
box = Box()
print(box.width) # 100
box.width = 10
print(box.width) # 10

# Mas seus valores originais ainda serão salvos nos atributos da classe
print(Box.width) # 100

```

### Exemplo B

```python
Box = namedtuple('Box', ('width', 'height', 'weight'))
box = Box(100, 200, 80)
print(box.width) # 100

# Tuplas são imutáveis, então esta é mais uma forma de agrupar constantes
box.width = 10 # AttributeError: can't set attribute
```

## Golang

### Exemplo A

```golang
func RetornaUmaPersonalidade(w http.ResponseWriter, r *http.Request) {
    id := 10

    for _, personalidade := range models.Personalidades {
        if strconv.Itoa(personalidade.Id) == id {
            json.NewEncoder(w).Encode(personalidade)
        }
    }
```

### Exemplo B

```golang
func RetornaUmaPersonalidade(w http.ResponseWriter, r *http.Request) {
    vars := mux.Vars(r)
    id := vars["id"]

    for _, personalidade := range models.Personalidades {
        if strconv.Itoa(personalidade.Id) == id {
            json.NewEncoder(w).Encode(personalidade)
        }
    }
```
