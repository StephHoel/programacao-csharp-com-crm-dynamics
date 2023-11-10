# Verificação de Idade

## Descrição

Você está desenvolvendo uma funcionalidade de verificação de idade para acesso ao CRM da sua empresa. A ferramenta verificará se um usuário é maior de idade para acessar determinados recursos.

**Funcionalidades:**

  - O programa começará solicitando a idade do usuário.
  - Ele verificará se o usuário tem 18 anos ou mais.
  - Se o usuário for maior de 18 anos, permitirá o acesso; caso contrário, negará o acesso.

**Instruções:**

  1. Solicite ao usuário que insira a idade.
  2. Use uma estrutura condicional if e else para verificar se a idade é maior ou igual a 18 anos.
  3. Exiba uma mensagem informando se o usuário tem ou não acesso permitido.

## Entrada

A entrada deverá ser realizada através do Console.ReadLine(), recebendo a seguinte informação:

  - A idade do usuário.

## Saída

A saída deverá retornar um texto informando:

  - Uma mensagem informando se o acesso é permitido ou negado.

## Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

| Entrada | Saída |
| - | - |
| 25 | Seja bem-vindo!<br>Acesso permitido ao CRM. |
| 16 | Acesso negado. Você não tem idade suficiente para acessar o CRM. |
| 44 | Seja bem-vindo!<br>Acesso permitido ao CRM. |

## Resultado

```csharp
using System;
using System.Collections.Generic;

public class HelloWorld
{
    public static void Main(string[] args)
    {
        int idade = int.Parse(Console.ReadLine());
        
        // TODO: Faça a verificação se o usuário é maior ou igual a 18 anos e imprima a mensagem exigida
        if (idade >= 18)
        {
            Console.WriteLine("Seja bem-vindo!\nAcesso permitido ao CRM.");
        }
        else
        {
            Console.WriteLine("Acesso negado. Você não tem idade suficiente para acessar o CRM.");
        }

    }
}
```