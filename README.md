#💻 Design Patterns in .NET 6

## 📜 Descrição

Este repositório demonstra a implementação de Design Patterns (Padrões de Projeto) utilizando .NET 6. O projeto abrange padrões criacionais, estruturais e comportamentais, e tem como objetivo mostrar como aplicar esses conceitos para resolver problemas comuns de software de maneira elegante e reutilizável.

Os padrões de design ajudam a criar sistemas mais flexíveis, fáceis de manter e escaláveis. Aqui, você encontrará explicações concisas de diversos padrões que podem ser usados em várias situações durante o desenvolvimento de software.

## 🚀 Padrões de Design Implementados

### 1. Padrões Criacionais 🛠️

Estes padrões lidam com a criação de objetos, abstraindo o processo de instanciamento.

**Singleton**

Garante que uma classe tenha apenas uma instância e fornece um ponto global de acesso a ela. Usado quando se deseja controlar o acesso a recursos compartilhados (como uma conexão com banco de dados).

**Factory Method**

Define uma interface para criar objetos, mas permite que as subclasses decidam qual classe instanciar. Usado quando a criação de um objeto é complexa ou depende de diferentes condições.

**Abstract Factory**

Permite a criação de famílias de objetos relacionados sem especificar suas classes concretas. Usado quando se trabalha com diferentes variantes de produtos que precisam ser criados de forma consistente.

**Builder**

Permite a criação de objetos complexos passo a passo, proporcionando flexibilidade e controle sobre o processo de construção. Usado quando um objeto tem muitas propriedades ou precisa ser configurado em etapas.

**Prototype**

Permite a criação de novos objetos duplicando um objeto existente (clonagem). Usado quando a criação de um objeto é cara ou complexa e pode ser melhorada pela clonagem de um protótipo.

#### 2. Padrões Estruturais 📐

Esses padrões lidam com a composição de objetos e classes para formar estruturas maiores e mais complexas.

**Adapter**

Permite que interfaces incompatíveis trabalhem juntas. Usado quando você precisa integrar dois sistemas com interfaces diferentes, adaptando uma para a outra sem modificar os sistemas originais.

**Bridge**

Desacopla uma abstração de sua implementação para que ambas possam variar independentemente. Usado quando se tem uma classe com várias funcionalidades que podem ser modificadas sem afetar as demais.

**Composite**

Permite que objetos individuais e composições de objetos sejam tratados de maneira uniforme. Usado para trabalhar com estruturas de objetos hierárquicas, como árvores (exemplo: pastas e arquivos).

**Decorator**

Adiciona comportamento adicional a um objeto de forma flexível e dinâmica, sem alterar sua estrutura. Usado quando você deseja estender as funcionalidades de um objeto de forma transparente e sem modificar o código original.

**Facade**

Fornece uma interface simplificada para um sistema complexo. Usado quando você precisa simplificar a interação com um sistema ou subsistema que tem muitas partes complexas.

**Flyweight**

Usa o compartilhamento de objetos para suportar grandes quantidades de objetos de forma eficiente. Usado quando você tem muitos objetos semelhantes e quer reduzir o uso de memória, compartilhando a mesma instância quando possível.

**Proxy**

Controla o acesso a um objeto, podendo adicionar lógica extra antes ou depois da chamada real. Usado quando você deseja controlar o acesso a um objeto de maneira transparente, como em casos de lazy loading ou controle de segurança.

### 3. Padrões Comportamentais 🔄

Esses padrões lidam com a interação e comunicação entre objetos, além de como os objetos se comportam e reagem a mudanças.

**Chain of Responsibility**

Permite que múltiplos objetos tratem uma requisição sem que o remetente saiba qual objeto irá tratá-la. Usado em sistemas onde uma solicitação pode ser processada por múltiplos manipuladores, como em pipelines de processamento.

**Command**

Encapsula uma solicitação como um objeto, permitindo parametrizar os clientes com diferentes solicitações. Usado para implementar funcionalidades de undo/redo, filas de tarefas, ou quando você deseja desacoplar os responsáveis pela execução de uma ação.

**Interpreter**

Define uma representação gramatical para uma linguagem e fornece um interpretador para processar a linguagem. Usado quando você precisa interpretar uma linguagem ou expressão complexa, como em compiladores ou parsers de linguagens de domínio específico.

**Iterator**

Permite acessar os elementos de um agregado de objetos sequencialmente, sem expor sua estrutura interna. Usado para navegar em coleções de objetos sem precisar conhecer sua implementação interna (exemplo: listas, árvores, etc.).

**Mediator**

Define um objeto que encapsula a comunicação entre objetos, evitando a dependência direta entre eles. Usado quando você tem múltiplos objetos que precisam se comunicar, mas deseja evitar que cada um se conecte diretamente aos outros.

**Memento**

Captura e externaliza o estado interno de um objeto, permitindo que o objeto possa ser restaurado para esse estado mais tarde. Usado para implementar funcionalidades como o histórico de mudanças, onde você precisa reverter para um estado anterior.

**Observer**

Define uma dependência um-para-muitos entre objetos, de forma que quando um objeto mudar de estado, todos os seus dependentes sejam notificados. Usado em sistemas que necessitam de notificação em tempo real, como em interfaces gráficas ou sistemas de eventos.

**State**

Permite que um objeto altere seu comportamento quando seu estado interno mudar. Usado quando um objeto deve alterar seu comportamento dependendo do seu estado atual, como um "semáforo" que muda entre estados de "vermelho", "amarelo" e "verde".

**Strategy**

Define uma família de algoritmos, encapsula cada um e os torna intercambiáveis. Usado quando você tem várias formas de executar uma ação e deseja escolher qual usar em tempo de execução, sem modificar o código que a utiliza.

**Template Method**

Define o esqueleto de um algoritmo, deixando alguns passos para que as subclasses os implementem. Usado para definir a estrutura de um algoritmo, onde alguns detalhes podem ser deixados para implementação específica das subclasses.

**Visitor**

Permite adicionar novas operações a objetos de uma estrutura sem modificar essas classes. Usado quando você precisa adicionar novas funcionalidades a objetos existentes sem alterar o código original, ideal para quando você tem uma estrutura de objetos complexa e precisa de extensões.

## 🛠️ Tecnologias

.NET 6 (C#)
XUnit (para testes unitários)
NUnit (para testes unitários, como alternativa)
Moq (para criação de mocks em testes)
FluentAssertions (para asserções fluentes nos testes)
Dependency Injection (usando o contêiner de DI do .NET)

## 🧑‍💻 Requisitos

**Pré-requisitos:**

.NET 6 SDK ou superior.
Editor de código como Visual Studio 2022 ou Visual Studio Code.

## 🚀 Como Usar

Clonando o Repositório

```
git clone https://github.com/usuario/design-patterns-dotnet6.git
cd design-patterns-dotnet6
```

Executando o Projeto

Compile o projeto:

```
dotnet build
```
Execute os testes:

```
dotnet test
```

Rode a aplicação de exemplo (se houver algum exemplo de execução de código):

```
dotnet run
```

## 🤝 Contribuição

Se você deseja contribuir com melhorias ou novas implementações, siga estas etapas:

Faça um fork do repositório.
Crie uma nova branch para sua feature (git checkout -b minha-feature).
Realize as alterações desejadas e faça commit (git commit -am 'Adiciona nova feature').
Envie suas alterações para o repositório remoto (git push origin minha-feature).
Abra um pull request explicando suas mudanças.

## 📝 Licença

Este projeto está licenciado sob a MIT License - veja o arquivo LICENSE.
