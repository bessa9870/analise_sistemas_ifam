# ANÁLISE DE SISTEMAS (Continuação)

## Documentação de casos de uso:

### Formatos de casos de uso principais
  1. Resumido: Um parágrafo apenas com o cenário principal;
  2. Completo: Várias sessões: interessados (usuários que se beneficiarão das funcionalidades do sistema) e interesses (funcionalidades do sistema, cadastros, registros...), pré-condições e pós-condições. Cenário principal e sequências alternativas.

### Dos tipos
  1. Abstrato: Utilizado na análise de requisitos sem muitos detalhes;
  2. Concreto: Utilizado na fase de projeto com mais detalhes.

### Exemplo de documentação de casos de uso resumidos
| **Caso de uso:** Emprestar livro |
|      :--      |
| **Visão geral:** A atendente da biblioteca realiza o empréstimo de um ou mais 
livros a um leitor apto a emprestar. O empréstimo é válido por um tempo determinado. | 

### Exemplo de documentação de casos de uso completo
| **Caso de uso:** |
| VisualizarProjeto |
|        :--        |
| **ID:** |
| UC9.3 |
| **Atores:** |
| Depart. Gerencial, professor e técnico administrativo |
| **Pré-condições:** |
|  1. O usuário deve estar logado no sistema; |
|  2. O usuário deverá ter a permissão a essa funcionalidade do sistema. |
| **Fluxo de eventos:** |
|  1. O usuário informa os dados necessários de acordo com o filtro estipulado; |
|  2. O sistema realiza busca por informações de acordo com os dados fornecidos; |
|  3. Se o sistema encontrar a informação: |
|       3.1. Para cada dado o sistema informa a informação; |
|       3.2. O sistema informa que não conseguiu encontrar nada. |
| **Pós-condições:** Nenhuma |
---
## Associações:
Representam as associações/relacionamentos entre:
  1. Atores e atores;
  2. Atores e casos de uso;
  3. Casos de uso e casos casos de uso.
Entre os casos:
  - Inclusão;
  - Extensão;
  - Generalização. 

### Associação `include` entre casos de uso
  Quando um caso de uso possui um comportamento parcial comum a vários casos de uso.
  ex: Caso **Movimentar conta** -> caso **Depositar** e caso **Sacar**

### Associação `extend` entre casos de uso
  É usado para descrever cenários opcionais de um caso de uso.
  ex: Realizar saque/Realizar depósito -> pode -> VIzualisar a conta

### Especialização/Generalização entre casos de uso
Forma de associação entre casos onde existem dois ou mais casos de uso com características semelhantes:
  *Três elipses ligadas por setas: "Abertura de conta", "Abertura de conta especial" e "Abertura de conta poupança".* 

### Associação entre o ator e o caso de uso
Demostra a ação que o ator utiliza do sistema representando essa ação no caso de uso:
  *Um boneco e uma elipse escrita "abertura de conta".*
      
### Especialização/Generalização entre atores
*Três bonecos ligados por setas: "Pessoa física" -> "Pessoa" <- "Pessoa jurídica".*

### Relacionamentos entre casos de uso
Existem casos em que a execução de um caso de uso implique a execução de outro um caso de uso pode ter uma parte que se repete em outro... Para evitar redundâncias, podemos isolar essas partes em casos de uso distintos e relacioná-los aos outros.
---
## DIAGRAMA DE CLASSES:
É o diagrama mais importante na UML, ele traz representações das abstrações das classes e relacionamentos mais importantes para o sistema. Definirá a arquitetura estático do sistema e servirá como base para a criação de novos diagramas futuros.
O diagrama é marcado pela **persistência de objetos das classes** a preservação permanente dos atributos de uma classe. É bem semelhante as entidades definidas com tabelas no banco de dados.

### Elementos do diagrama de classes
  - Classes;
  - Relacionamentos.
        - Associação - relação de utilização.
            - Associativa unária;
            - Associação binária;
            - Associação ternária;
            - Agregação;
            - Composição.
        - Generalização - relação de herança;
        - Dependência;
        - Realização;
        - Classe associativa;
        - Restrição.
    - Atributos.
    - Operações/métodos
          - Descrevem o comportamento da classe.

| **Nome da entidade** |
| NotaFiscal |
|   :--   |
| **Atributos** |
|-codigo |
|-naturezaOperacao |
|-condicaoPagamento |
|-tipoPrestServico |
|-dataEmissao |
|- valor |
| **Operações** |
|+registrar() |
|+recuperar() |
|+cancelar() |

### Visibilidade dos atributos e métodos
Temos as seguintes possibilidades para visibilidade nas operações:
**Pública: (+)** A operação é visível para elementos no modelo;
**Protegida: (#)** A operação é visível somente para a classe e suas subclasses ou para **amigos** da classe dependendo do modelo;
**Privada: (-)** A operação é visível somente para a classe e **amigos** da classe dependendo do modelo.

### Os identificadores da classe
Refere normalmente a objetos concretos, mas deve abstrair a realidade e encontrar descrições adequadas a vários objetos semelhantes. (não entendi nada)

### Identificando classes
  - Identificação de entidades;
  - Identificação de atributos;
  - Identificação de operações;
  - Identificação de relacionamentos;

*nomes*
### Identificação de entidades
Permitir representar elementos do mundo real dentro do mundo computacional através da abstração. Pode-se procurar na especificação dos casos de uso por conceitos que representem objetos do domínio de aplicação a ser desenvolvida.

### Identificação de atributos
Propriedades que caracterizam um objeto. Atributos devem estar alinhados com as necessidades do usuário para o problema. Os nomes devem ser significativos e, se necessário, identificar a visibilidade dos atributos
  - (+) Públicos;
  - (-) Privados;
  - (#) Protegidos;

### Identificação de operações (métodos/serviços)
São ações que o indivíduo é capaz de efetuar. Deve identificar ações que o objeto de uma classe é responsável e pode desempenhar dentro do escopo do sistema que será desenvolvido. Normalmente, operações são públicas e tem sua utilização por outros objetos também.

### Identificação de relacionamentos
Último passo na construção de um diagrama de classes e a parte mais complicada.

### Associações
Permite especificar quais objetos de uma classe se relacionam com objetos de outra classe.

### Associação unária
Ocorre quando existe um relacionamento de uma classe consigo mesma.

### Associação binária
Uma relação estrutural entre duas classes, onde duas classes trocam mensagens.
ex: ContaBancaria <1-1> Cliente. Socio <N-N> Dependente; 

### Associação ternária
Úteis para associações complexas, leitura difícil de se interpretar.
ex:
            Turma
Professor-----<>
           SalaDeAula

### Associação de agregação
Demonstra que as informações de um objeto (objeto-todo) precisam ser complementadas pelas informações em outro ou outros objetos de outras classes (objeti-parte). Um objeto parte não pode ser destruído por um objeto diferente do objeto-todo.

ex:
Agencia <>----ContaBancaria
