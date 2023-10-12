# Desafios Java: Abrindo Contas

# ****Desafio****

Você é um desenvolvedor em início de carreira e foi contratado por um banco para criar um sistema básico de abertura de contas. Sua tarefa é implementar uma classe chamada "ContaBancaria" que represente uma conta bancária com as seguintes informações: número da conta, nome do titular e saldo.

# ****Entrada****

O programa deve solicitar ao usuário as informações necessárias para abrir uma conta bancária. A entrada deve ser feita via console (linha de comando) e deve incluir o número da conta (um valor inteiro), o nome do titular (uma sequência de caracteres) e o saldo inicial da conta (um valor decimal).

# Saída

Após receber as informações da conta, o programa deve criar um objeto do tipo "ContaBancaria" e exibir na tela as informações dessa conta, incluindo o número da conta, o nome do titular e o saldo atual. A saída deve ser formatada de forma clara e legível para o usuário.

# Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.

| Entrada | Saída |
| --- | --- |
| 010101 <br> Caio Carlos <br> 98.0 <br> | Informacoes: <br> Conta: 101010 <br> Titular: Caio Carlos <br> Saldo: R$ 98.0 <br> |
|212223 <br> Carla Paiva <br> 500.0 <br> | Informacoes: <br> Conta: 212223 <br> Titular: Carla Paiva <br> Saldo: R$ 500.0 <br> |
| 123456 <br> Joao Silva <br> 1000.0 <br>| Informacoes: <br> Conta: 123456 <br> Titular: Joao Silva <br> Saldo: R$ 1000.0 <br> |

# Solução:

```java
import java.util.Scanner;

public class Desafio {

  public static void main(String[] args) {
    // Lendo os dados de Entrada:
    Scanner scanner = new Scanner(System.in);
    int numeroConta = scanner.nextInt();
    scanner.nextLine(); // Consome a quebra de linha após a entrada do número da conta
    String nomeTitular = scanner.nextLine();
    double saldo = scanner.nextDouble();

    //TODO: Criar uma instância de "ContaBancaria" com os valores de Entrada.

    System.out.println("Informacoes:");
    //TODO: Imprimir as informações da conta usando o objeto criado no TODO acima.
  }
}

class ContaBancaria {
  int numero;
  String titular;
  double saldo;

  public Bancaria(int numero, String titular, double saldo) {
    this.numero = numero;
    this.titular = titular;
    this.saldo = saldo;
  }
}
```