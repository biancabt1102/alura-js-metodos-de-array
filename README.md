# JavaScript: Métodos com Array

## O que estou aprendendo?

### map()
Ele invoca a função passada por argumento para cada elemento do array e **devolve** um novo Array como resultado. Por exemplo:

```
    const array1 = [1, 4, 9, 16];

    // Pass a function to map
    const map1 = array1.map(x => x * 2);

    console.log(map1);
    // Expected output: Array [2, 8, 18, 32]
```

### Reticências (...)
Ele vai fazer uma copia de um array, ou do objeto existente, para um outro objeto.

### forEach()
Manipula os dados reais de um array.

### filter()
Filtra um array e cria um novo array.

```
    const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];

    const result = words.filter(word => word.length > 6);

    console.log(result);
    // Expected output: Array ["exuberant", "destruction", "present"]
```

### sort()
Ele ordena os elementos de acordo com a pontuação de código Unicode.

```
    const months = ['March', 'Jan', 'Feb', 'Dec'];
    months.sort();
    console.log(months);
    // Expected output: Array ["Dec", "Feb", "Jan", "March"]

    const array1 = [1, 30, 4, 21, 100000];
    array1.sort();
    console.log(array1);
    // Expected output: Array [1, 100000, 21, 30, 4]

```

Mas para fazer uma ordenação de menor para maior ou vice-versa tem que ser criada uma função.

### reduce()
Executa uma função reducer para cada elemento do array, resultando num único valor de retorno.
```
    const array1 = [1, 2, 3, 4];

    // 0 + 1 + 2 + 3 + 4
    const initialValue = 0;
    const sumWithInitial = array1.reduce(
    (accumulator, currentValue) => accumulator + currentValue,
    initialValue
    );

    console.log(sumWithInitial);
    // Expected output: 10
```
Parâmetros:  
1. Acumulador (acc)
2. Valor Atual (cur)
3. Index Atual (idx)
4. Array original (src)

## Diferença entre map(), filter() e reduce()

![Imagem explicando a diferença](https://miro.medium.com/max/785/1*yD7P1I36G1jTProLQwEXxA.jpeg)