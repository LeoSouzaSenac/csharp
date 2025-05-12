## ✅ Aula 1: Conceitos Básicos de C\#

### 🎯 Objetivo

* Instalar o ambiente de desenvolvimento
* Entender a estrutura básica de um programa em C#
* Aprender os principais **tipos de dados**, **variáveis**, **constantes**, **operadores** e **estruturas de controle** (condicionais e laços)

---

### 🛠️ Instalação e Configuração do Ambiente

#### Opção 1: Visual Studio (Completo)

1. Baixe o Visual Studio Community 2022 (gratuito):
   [https://visualstudio.microsoft.com/pt-br/](https://visualstudio.microsoft.com/pt-br/)
2. Durante a instalação, selecione **"Desenvolvimento para desktop com .NET"**

#### Opção 2: Visual Studio Code (mais leve)

1. Instale o VS Code: [https://code.visualstudio.com/](https://code.visualstudio.com/)
2. Instale o .NET SDK: [https://dotnet.microsoft.com/download](https://dotnet.microsoft.com/download)
3. No terminal, verifique se está instalado:

   ```bash
   dotnet --version
   ```
4. Instale a extensão "C#" no VS Code

---

### 📄 Estrutura de um Programa em C\#

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Olá, mundo!");
    }
}
```

* `using System;`: importa funcionalidades básicas, como Console
* `Main`: ponto de entrada da aplicação
* `Console.WriteLine`: imprime na tela

---

### 🔠 Tipos de Dados

| Tipo     | Exemplo                | Descrição           |
| -------- | ---------------------- | ------------------- |
| `int`    | `int idade = 30;`      | Números inteiros    |
| `double` | `double pi = 3.14;`    | Números decimais    |
| `bool`   | `bool ativo = true;`   | Verdadeiro ou falso |
| `string` | `string nome = "Ana";` | Texto               |
| `char`   | `char letra = 'A';`    | Um único caractere  |

---

### 📦 Variáveis e Constantes

```csharp
int idade = 25;
const double PI = 3.1415;
string nome = "Carlos";
```

* `const`: valor que não pode ser alterado
* Use nomes significativos e camelCase para variáveis

---

### ➕ Operadores

#### Aritméticos

```csharp
+ - * / %
```

#### Relacionais

```csharp
== != > < >= <=
```

#### Lógicos

```csharp
&& (E)   || (OU)   ! (NÃO)
```

---

### 🔁 Estruturas de Controle

#### Condicional `if`, `else`, `else if`

```csharp
int idade = 18;
if (idade >= 18)
{
    Console.WriteLine("Maior de idade");
}
else
{
    Console.WriteLine("Menor de idade");
}
```

#### `switch`

```csharp
int opcao = 2;
switch (opcao)
{
    case 1:
        Console.WriteLine("Opção 1");
        break;
    case 2:
        Console.WriteLine("Opção 2");
        break;
    default:
        Console.WriteLine("Opção inválida");
        break;
}
```

---

### 🔁 Estruturas de Repetição

#### `for`

```csharp
for (int i = 0; i < 5; i++)
{
    Console.WriteLine("Contagem: " + i);
}
```

#### `while`

```csharp
int i = 0;
while (i < 5)
{
    Console.WriteLine("i: " + i);
    i++;
}
```

#### `do-while`

```csharp
int i = 0;
do
{
    Console.WriteLine("Valor: " + i);
    i++;
} while (i < 5);
```

#### `foreach`

```csharp
string[] nomes = { "Ana", "Lucas", "Pedro" };
foreach (string nome in nomes)
{
    Console.WriteLine(nome);
}
```

---

## 🧪 Exercícios

1. Crie um programa que leia um nome e idade e imprima:
   **"Olá, \[nome], você tem \[idade] anos."**

2. Crie um programa que pergunte se a pessoa quer continuar (S/N).
   Se digitar "S", imprima **"Você escolheu continuar!"**.

3. Crie um `for` que conte de 1 a 10.

4. Crie um programa que peça um número e diga se é **par ou ímpar**.

