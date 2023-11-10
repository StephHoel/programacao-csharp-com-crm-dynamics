# Gerenciamento de Contatos

## Descrição

O Dynamics 365 é uma poderosa ferramenta de gerenciamento de relacionamento com o cliente usada por empresas para rastrear, armazenar e interagir com contatos, como clientes, leads e parceiros de negócios. Sua tarefa é criar um programa que permita a um usuário adicionar informações de contato ao Dynamics 365 e classificar esses contatos em categorias específicas

## Entrada

A entrada deverá ser realizada através do Console.ReadLine(), recebendo as seguintes informações:

    - Nome do contato (uma string).
    - Endereço de e-mail do contato (uma string).
    - Número de telefone do contato (uma string).

## Saída

A saída deverá retornar um texto informando:

    - A Confirmação de que o contato foi adicionado com sucesso.
    - Exibição das informações do contato, incluindo nome, endereço de e-mail e número de telefone.

## Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

| Entrada | Saída |
| - | - |
| Joao<br>j@dio.com<br>123432 | Contato adicionado!<br>Nome: Joao<br>E-mail: j@dio.com<br>Tel: 123432 |
| Ana<br>ana@email.com<br>010101 | Contato adicionado!<br>Nome: Ana<br>E-mail: ana@email.com<br>Tel: 010101 |
| Rafa<br>rafa@dio.com<br>555000 | Contato adicionado!<br>Nome: Rafa<br>E-mail: rafa@dio.com<br>Tel: 555000 |

## Resposta

```csharp
using System;

public class HelloWorld
{
    public static void Main(string[] args)
    {
        while (true)
        {

            string nome = Console.ReadLine();


            string email = Console.ReadLine();


            string telefone = Console.ReadLine();

            // TODO: Exiba a confirmação de que o contato foi adicionado com sucesso
            
            Console.WriteLine("Contato adicionado!");
           
            // TODO: Exiba as informações do contato
            
            Console.WriteLine("Nome: " + nome);
            Console.WriteLine("E-mail: " + email);
            Console.WriteLine("Tel: " + telefone);

            
            break;
        }
    }
}
```
