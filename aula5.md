# ANÁLISE DE SISTEMAS (Continuação)

## Documentação de casos de uso:

### Formatos de casos de uso principais:
  1. Resumido: Um parágrafo apenas com o cenário principal;
  2. Completo: Várias sessões: interessados (usuários que se beneficiarão das funcionalidades do sistema) e interesses (funcionalidades do sistema, cadastros, registros...), pré-condições e pós-condições. Cenário principal e sequências alternativas.

### Dos tipos:
  1. Abstrato: Utilizado na análise de requisitos sem muitos detalhes;
  2. Concreto: Utilizado na fase de projeto com mais detalhes.

### Exemplo de documentação de casos de uso resumidos:
| **Caso de uso:** Emprestar livro |
|      :--      |
| **Visão geral:** A atendente da biblioteca realiza o empréstimo de um ou mais 
livros a um leitor apto a emprestar. O empréstimo é válido por um tempo determinado. | 

### Exemplo de documentação de casos de uso completo:
| **Caso de uso:** VisualizarProjeto |
|        :--        |
| **ID:** UC9.3 |
| **Atores:** Depet. Gerec, professor e técnico administrativo |
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

### Associação entre o ator e o caso de uso:
Demostra a ação que o ator utiliza do sistema representando essa ação no caso de uso:
  *Um boneco e uma elipse escrita "abertura de conta".*

### Especialização/Generalização entre casos de uso:
Forma de associação entre casos onde existem dois ou mais casos de uso com características semelhantes:
  *Três elipses ligadas por setas: "Abertura de conta", "Abertura de conta especial" e "Abertura de conta poupança".* 
      
### Especialização/Generalização entre atores:
*Três bonecos ligados por setas: "Pessoa física" -> "Pessoa" <- "Pessoa jurídica".*

### Relacionamentos entre casos de uso:
Existem casos em que a execução de um caso de uso implique a execução de outro um caso de uso pode ter uma parte que se repete em outro... Para evitar redundâncias, podemos isolar essas partes em casos de uso distintos e relacioná-los aos outros.

**Associação <<include>>**
  Quando um caso de uso possui um comportamento parcial comum a vários casos de uso.
  ex: Caso **Movimentar conta** -> **Depositar/Sacar**

**Associação <<extend>>
  É usado para descrever cenários opcionais de um caso de uso.
  ex: Realizar saque/Realizar depósito -> pode -> VIzualisar a conta
