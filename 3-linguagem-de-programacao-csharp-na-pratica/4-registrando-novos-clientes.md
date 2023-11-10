# Registrando Novos Clientes

## Descrição

Imagine que você está desenvolvendo uma aplicação de registro de novos clientes para uma empresa que utiliza o Dynamics 365 para gerenciar seus relacionamentos com os clientes. O objetivo é criar uma ferramenta simples que permita aos funcionários registrar informações dos clientes no sistema Dynamics 365 de forma eficaz.

## Entrada

A entrada será realizada através do Console.ReadLine(). O programa solicitará ao usuário que insira as seguintes informações do cliente, uma por vez:

  - Nome do cliente.
  - Endereço de e-mail do cliente.
  - Número de telefone do cliente.

Após cada entrada, o programa perguntará se o usuário deseja continuar registrando clientes (digitando "S" para sim ou "N" para não).

## Saída

A saída deverá:

  - Exibir as informações do cliente registrado, incluindo nome, endereço de e-mail e número de telefone.

Se o usuário decidir parar de registrar clientes, o programa exibirá as informações de todos os clientes registrados até o momento. 

## Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

|Entrada | Saída |
| - | - |
| Gabriel<br>ga@email.com<br>123-432<br>N | Gabriel, g@email.com, 123-432 |
| Lia<br>lia@test.com<br>033-444<br>S<br>Ana<br>ana@gmail.com<br>111-111<br>N | Lia, lia@test.com, 033-444<br>Ana, ana@gmail.com, 111-111 |
| Ju<br>j@email.com<br>999-999<br>S<br>Bru<br>bru@dio.me<br>111-222<br>S<br>Leo<br>l@gmail.com<br>555-555<br>N | Ju, j@email.com, 999-999<br>Bru, bru@dio.me, 111-222<br>Leo, l@gmail.com, 555-555|

## Resultado

```csharp
using System;
using System.Collections.Generic;

public class HelloWorld
{
    public static void Main(string[] args)
    {
        List<string> clientes = new List<string>();
        
        string continuar = "S";

        while (continuar == "S")
        {
            string nome = Console.ReadLine();
            string email = Console.ReadLine();
            string telefone = Console.ReadLine();

            // Registra o cliente (simulação)
            string clienteInfo = $"{nome}, {email}, {telefone}";
            clientes.Add(clienteInfo);

            continuar = Console.ReadLine();

            // TODO: Adicione uma condição para verificar se o usuário deseja continuar registrando mais clientes e, se desejar, continuar o loop para coletar mais informações.
        
          
        }
        
          foreach(string client in clientes){
            Console.WriteLine(client);
          }
        
    }
}
```
