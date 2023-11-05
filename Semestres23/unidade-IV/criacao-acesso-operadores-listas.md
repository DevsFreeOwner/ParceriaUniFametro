## JAVASCRIPT

### Exemplo

> index.js
```javascript
//Importa style.css
import './style.css';

function math(strings, x, y) {
  // TODO: constrói árvore de expressão a partir de valores e strings
  // por enquanto a implementação abaixo assume um expresso
  // com um único operador binário de um subconjunto específico.

  const operator = strings[1].replace(/\s/gi, "");
  
  if (operator == "∘") {
    return x + 2 * y;
  }
  else if (operator == "^") {
    return Math.trunc(x, y);
  }
  else {
    return `Operador desconhecido '${operator}'`;
  }
}

// Escreva o código Javascript!
const appDiv = document.getElementById('app');
appDiv.innerHTML = math`${2} ∘ ${2}`;
```

> index.html
```html
<div id="app"></div>
```

> style.css
```css
style.css
h1, h2 {
  font-family: Lato;
}
```

### Os Melhores IDEs pelo navegador

- vscode.dev
- AWS Cloud9
- CodeTasty
- Codeacademy
-  p5.js
- Codevny
- JSFiddle
- Gitpod
- Repl.it
- Codepen.io
- Small Basic
- Arduino Web Editor
- XOD.io