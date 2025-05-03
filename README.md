# 📚 Métodos de Arrays em JavaScript

Este repositório contém uma lista completa dos principais métodos de arrays do JavaScript com exemplos comentados para consulta e estudo.

---

## 🔍 Métodos de Busca e Filtro

### `.find()`

Procura o **primeiro** elemento que satisfaça a condição.

```js
[10, 20, 30].find(n => n > 15); // 👉 20
```

### `.filter()`

Filtra **todos** os elementos que satisfazem a condição.

```js
[10, 20, 30].filter(n => n > 15); // 👉 [20, 30]
```

### `.findIndex()`

Retorna o índice do primeiro elemento que satisfaz a condição.

```js
[10, 20, 30].findIndex(n => n > 15); // 👉 1
```

### `.includes()`

Verifica se um valor existe no array.

```js
[1, 2, 3].includes(2); // 👉 true
```

### `.indexOf()`

Retorna o índice da **primeira ocorrência** de um valor.

```js
[1, 2, 3, 2].indexOf(2); // 👉 1
```

### `.lastIndexOf()`

Retorna o índice da **última ocorrência** de um valor.

```js
[1, 2, 3, 2].lastIndexOf(2); // 👉 3
```

---

## 🔄 Métodos de Transformação

### `.map()`

Transforma cada item do array e retorna um novo array.

```js
[1, 2, 3].map(n => n * 2); // 👉 [2, 4, 6]
```

### `.reduce()`

Reduz o array a um único valor acumulado.

```js
[1, 2, 3].reduce((acc, n) => acc + n, 0); // 👉 6
```

### `.flat()`

Achata arrays aninhados em um único nível.

```js
[1, [2, 3], [4]].flat(); // 👉 [1, 2, 3, 4]
```

### `.flatMap()`

Aplica uma função e achata o resultado em um novo array.

```js
[1, 2, 3].flatMap(n => [n, n * 2]); // 👉 [1, 2, 2, 4, 3, 6]
```

---

## 🧪 Métodos de Verificação

### `.every()`

Verifica se **todos** os elementos satisfazem a condição.

```js
[2, 4, 6].every(n => n % 2 === 0); // 👉 true
```

### `.some()`

Verifica se **ao menos um** elemento satisfaz a condição.

```js
[1, 2, 3].some(n => n > 2); // 👉 true
```

---

## 🛠️ Métodos de Modificação (Mutáveis)

### `.push()`

Adiciona um elemento ao **final** do array.

```js
let a = [1, 2];
a.push(3); // 👉 [1, 2, 3]
```

### `.pop()`

Remove o último elemento do array.

```js
a.pop(); // 👉 [1, 2]
```

### `.unshift()`

Adiciona um elemento no **início** do array.

```js
a.unshift(0); // 👉 [0, 1, 2]
```

### `.shift()`

Remove o primeiro elemento do array.

```js
a.shift(); // 👉 [1, 2]
```

### `.splice()`

Adiciona, remove ou substitui elementos em qualquer posição.

```js
let b = [1, 2, 3];
b.splice(1, 1, "novo"); // 👉 [1, "novo", 3]
```

### `.sort()`

Ordena os elementos do array (por padrão como strings).

```js
let c = [5, 10, 1];
c.sort((a, b) => a - b); // 👉 [1, 5, 10]
```

### `.reverse()`

Inverte a ordem dos elementos.

```js
[1, 2, 3].reverse(); // 👉 [3, 2, 1]
```

---

## 📄 Outros Métodos Úteis

### `.slice()`

Retorna uma parte do array sem modificar o original.

```js
[1, 2, 3, 4].slice(1, 3); // 👉 [2, 3]
```

### `.join()`

Une todos os elementos do array em uma string.

```js
[1, 2, 3].join("-"); // 👉 "1-2-3"
```

### `.concat()`

Concatena dois ou mais arrays.

```js
[1, 2].concat([3, 4]); // 👉 [1, 2, 3, 4]
```

### `.forEach()`

Executa uma função para cada item do array.

```js
[1, 2, 3].forEach(n => console.log("forEach 👉", n));
```




