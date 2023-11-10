# Criando uma Lista de Contatos no CRM

## Descrição

Você está desenvolvendo uma ferramenta para criar uma lista de clientes no sistema CRM. A ferramenta permite ao usuário definir o tamanho da lista e, em seguida, inserir os nomes dos clientes.

**Funcionalidades:**

  - O programa solicitará ao usuário que defina o tamanho da lista de clientes.
  - Em seguida, o usuário será solicitado a inserir o nome de cada cliente na lista.
  - Depois de coletar os nomes, o programa usará um loop foreach para exibir todos os nomes dos clientes na lista.

**Instruções:**

  1. Solicite ao usuário que insira o tamanho da lista de clientes.
  2. Crie uma lista vazia para armazenar os nomes dos clientes.
  3. Use um loop for para coletar os nomes dos clientes de acordo com o tamanho definido.
  4. Use um loop foreach para exibir todos os nomes dos clientes na lista.

## Entrada

A entrada será realizada através do Console.ReadLine(). O programa solicitará ao usuário que insira as seguintes informações:

  - O tamanho da lista de clientes.
  - Os nomes dos clientes, um por vez, conforme solicitado

## Saída

A saída deverá retornar:

  - A lista de nomes dos clientes inseridos.

## Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

|Entrada | Saída |
| - | - |
| 1<br>Renato | Lista de Contatos:<br>1. Renato |
| 3<br>Camila<br>Felipe<br>Venilton | Lista de Contatos:<br>1. Camila<br>2. Felipe<br>3. Venilton |
| 2<br>Ana<br>Joana | Lista de Contatos:<br>1. Ana<br>2. Joana |

## Resultado

```csharp
using System;
using System.Collections.Generic;

public class HelloWorld
{
    public static void Main(string[] args)
    {

        int tamanhoLista = int.Parse(Console.ReadLine());

        List<string> listaClientes = new List<string>();

        for (int i = 1; i <= tamanhoLista; i++)
        {
            // TODO: Solicite ao usuário o nome do cliente e adiciona à lista
            listaClientes.Add(Console.ReadLine());
        }

        Console.WriteLine("\nLista de Contatos:");

        for (int i = 0; i < listaClientes.Count; i++)
        {
            //TODO: Exibe o número do cliente na lista e o nome do cliente
            Console.WriteLine(i+1 + ". " + listaClientes[i]);
        }
    }
}
```
