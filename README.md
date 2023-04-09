# Exemplo simples de Polimorfismo em C#.

## Descrição do código
* O código consiste em um console application que cria uma lista de três elementos e tenta cadastrar um texto na lista. O método de cadastro lança uma exceção personalizada caso o texto seja nulo ou vazio.

## Classes do projeto:

* Classe "Program":
* Esta é a classe principal do programa. Inclui o método Main, que cria os objetos Estagiario, Gerente e Atendente e chama seus respectivos métodos valeAlimentacao e valeTransporte. Esses métodos calculam e imprimem os descontos padrão de alimentação e transporte para cada funcionário.

* Classe "Imposto":
* Esta é uma classe abstrata que serve como base para todas as outras classes. Nela existem dois métodos: valeAlimentacao e valeTransporte. O método valeAlimentacao calcula e imprime o desconto padrão de alimentação, enquanto o método valeTransporte calcula e imprime o desconto padrão de transporte.

* Classe "Gerente":
* Esta é uma subclasse de Imposto. Substitui o método valeAlimentacao para calcular e imprimir um desconto diferenciado em alimentação para a classe Gerente.

* Classe "Atendente":
* Esta é uma subclasse de Imposto. Substitui o método valeAlimentacao para calcular e imprimir um desconto diferenciado em alimentação para a classe Atendente.

* Classe "Estagiário":
* Esta é uma subclasse de Imposto. Ele não sobrescreve nenhum método, então usa as implementações padrão da classe Imposto de valeAlimentacao e valeTransporte.

## Como executar o código
* Para executar o código, é necessário ter o ambiente de desenvolvimento .NET instalado na máquina. Para compilar e executar o código, basta seguir os seguintes passos:

* Abra um terminal e navegue até a pasta onde se encontra o arquivo Program.cs.
* Compile o código com o comando dotnet build.
* Execute o programa com o comando dotnet run.

## Tecnologia utilizada:

* [C#](https://docs.microsoft.com/pt-br/dotnet/csharp/): linguagem de programação 

