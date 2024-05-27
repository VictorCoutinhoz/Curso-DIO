# | Para resolver o desafio de criar o projeto ContaBanco, será necessário que a classe `ContaTerminal.java`, receba dados via terminal e exiba uma mensagem formatada com as informações inseridas pelo usuário. |
---
## Segui os seguintes passos para realizar a tarefa:

1. Criação do projeto ContaBanco.
2. Desenvolvimento da classe ContaTerminal.java.
3. Uso da classe Scanner para receber as informações do usuário.
4. Armazenamento das informações em variáveis adequadas.
5. Exibição da mensagem final com as informações concatenadas.
---
# Explicação do Código
1. Importação da Classe `Scanner`:
~~~java
import java.util.Scanner;
~~~
2. Criação do Método `main`:
~~~java
public static void main(String[] args) {
~~~
3. Define o ponto de entrada do programa.
Criação do Objeto Scanner:

~~~java
Scanner scanner = new Scanner(System.in);
~~~
Cria um objeto Scanner para ler a entrada do usuário.

4. Leitura do Número da Conta:

~~~java
System.out.println("Por favor, digite o número da Conta!");
int numero = scanner.nextInt();
scanner.nextLine(); // Consumir a nova linha deixada pelo nextInt()
~~~
Solicita e lê o número da conta. scanner.nextLine() é usado para consumir a nova linha deixada pelo nextInt().

5. Leitura da Agência:

~~~java
System.out.println("Por favor, digite o número da Agência!");
String agencia = scanner.nextLine();
~~~
Solicita e lê a agência como uma String.

6. Leitura do Nome do Cliente:

~~~java
System.out.println("Por favor, digite o nome do Cliente!");
String nomeCliente = scanner.nextLine();
~~~
Solicita e lê o nome do cliente.

7. Leitura do Saldo:

~~~java
System.out.println("Por favor, digite o saldo!");
double saldo = scanner.nextDouble();
~~~
Solicita e lê o saldo como um double.

## Exibição da Mensagem Final:

~~~java
System.out.println("Olá " + nomeCliente + ", obrigado por criar uma conta em nosso banco, sua agência é " + agencia + ", conta " + numero + " e seu saldo " + saldo + " já está disponível para saque.");
~~~
Exibe uma mensagem formatada com as informações inseridas.

Fechamento do Scanner:

~~~java
scanner.close();
~~~
Fecha o objeto Scanner para liberar os recursos associados a ele.

* _Este código cobre todos os requisitos do desafio, permitindo que o usuário insira informações via terminal e exibindo uma mensagem formatada com essas informações._