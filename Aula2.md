## ✅ Aula 2: Estruturas de Dados e Coleções

### 🎯 Objetivo

* Aprender como usar arrays, listas genéricas, tuplas e dicionários
* Entender quando usar cada estrutura de forma eficiente

---

## 🔢 1. Arrays

### 📌 O que é?

Um array é uma coleção fixa de elementos do mesmo tipo.

### 📘 Sintaxe

```csharp
int[] numeros = new int[3]; // Cria array com 3 posições
numeros[0] = 10;
numeros[1] = 20;
numeros[2] = 30;
```

### 📘 Inicialização direta

```csharp
string[] nomes = { "Ana", "Lucas", "Maria" };
Console.WriteLine(nomes[1]); // Lucas
```

---

### 🔄 Percorrer com `for` ou `foreach`

```csharp
foreach (string nome in nomes)
{
    Console.WriteLine(nome);
}
```

---

### 🔢 Arrays Multidimensionais

```csharp
int[,] matriz = new int[2, 2];
matriz[0, 0] = 1;
matriz[0, 1] = 2;
matriz[1, 0] = 3;
matriz[1, 1] = 4;

for (int i = 0; i < 2; i++)
{
    for (int j = 0; j < 2; j++)
    {
        Console.WriteLine(matriz[i, j]);
    }
}
```

---

## 📋 2. Listas Genéricas (`List<T>`)

### 📌 O que é?

Uma lista que **cresce dinamicamente** e permite adicionar/remover elementos.

### 📘 Exemplo:

```csharp
using System.Collections.Generic;

List<string> frutas = new List<string>();
frutas.Add("Maçã");
frutas.Add("Banana");
frutas.Add("Laranja");

foreach (string fruta in frutas)
{
    Console.WriteLine(fruta);
}
```

### 🔍 Métodos úteis:

* `Add(valor)` – adiciona
* `Remove(valor)` – remove
* `Contains(valor)` – verifica existência
* `Count` – total de itens
* `Clear()` – limpa tudo

---

## 🔑 3. Dicionários (`Dictionary<TKey, TValue>`)

### 📌 O que é?

Armazena pares **chave-valor**.

### 📘 Exemplo:

```csharp
using System.Collections.Generic;

Dictionary<string, int> estoque = new Dictionary<string, int>();
estoque["Caneta"] = 10;
estoque["Lápis"] = 20;

Console.WriteLine("Canetas no estoque: " + estoque["Caneta"]);
```

### 🔍 Métodos úteis:

* `Add(chave, valor)`
* `Remove(chave)`
* `ContainsKey(chave)`
* `TryGetValue(chave, out valor)`
* `Keys`, `Values`

---

## 🧺 4. Tuplas

### 📌 O que é?

Permite retornar ou armazenar múltiplos valores com tipos diferentes.

### 📘 Exemplo:

```csharp
(string, int) produto = ("Caderno", 25);
Console.WriteLine($"Produto: {produto.Item1}, Quantidade: {produto.Item2}");
```

### 📘 Com nomes personalizados:

```csharp
var pessoa = (nome: "João", idade: 30);
Console.WriteLine($"Nome: {pessoa.nome}, Idade: {pessoa.idade}");
```

---

## 🧪 Exercícios

1. **Array**: Crie um array com 5 números inteiros e imprima a soma deles.
2. **List**: Crie uma lista de nomes. Adicione 3 nomes e depois remova 1. Mostre os nomes restantes.
3. **Dicionário**: Crie um dicionário com 3 produtos e seus preços. Permita que o usuário digite o nome de um produto e mostre o preço.
4. **Tupla**: Crie uma função que retorne uma tupla com o nome completo e idade de uma pessoa.
