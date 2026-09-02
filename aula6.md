## Como encontrar relações entre as classes identificadas 
**Agregação:** Verifica se a há alguma relação "parte de" entre as classes;

**Composição:** Verifica se há alguma relação "parte de" forte entre as classes;

**Navegação:** Verifica se existem navegações desnecessárias entre as classes;

**Classe associativa:** Verifica se existem informações que precisam estar vinculadas à associação entre dois objetos, mas não em um deles em particular.

## Estereótipos:
São maneiras de destacar/diferenciar um componentes/relacionamento de outros iguais, atribuindo-os características especiais ou as modificando de alguma forma.
  - Estereótipo de rótulo;
  - Estereótipo de gráfico

### Estereótipo `entity`
Torna explícito que uma classe é uma entidade. Logo, a classe contém informações recebidas ou geradas por meio do sistema. Classes desse estereótipo geralmente 
fornecem muitas informações objetos e terão um longo período de vida, estes objetos precisam ser preservados por meio da persistência de dados.

### Estereótipo `boundary`
Também conhecido como **Estereótipo de fronteira**. Esse estereótipo é importante quando se tem a necessidade de definir a existência de uma interface para o
sistema, empregando uma classe como meio de comunicação entre atores externos e o sistema além de possibilitar a comunicação com uma classe **control**.

### Estereótipo `control`
Identifica classes que servem de intermediadores entre as classes boundary com as demais do sistema. As classes control interpretam os eventos ocorrido sobre
os objetos boundary, como o movimento do mouse e um pressionamento de um botão e retransmite esses eventos (transcreve) para os objetos das classes de entidades
que compõem o sistema.
