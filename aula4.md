# ANÁLISE DE SISTEMAS

## DIAGRAMAS DA UML 2.0
*UML - Unified modeling language.* Por: Grady Booch

  - Diagrama de casos de uso;
  - Diagrama de classe;
  - Diagrama de objetos;
  - Diagrama de sequência;
  - Diagrama de comunicação;
  - Diagrama de Máquina de Estados;
  - Diagrama de Atividade;
  - Diagrama de Componentes;
  - Diagrama de Implantação;
  - Diagrama de Interação Geral;
  - Diagrama de Pacotes;
  - Diagrama de Tempo;
  - Diagrama de Estrutura Composta.

  Segundo **Edsger Dijkstra** Ataque um problema difícil em vários problemas menores para solucioná-los. Construímos modelos de sistemas complexos pois não somos capazes de compreendê-los totalmente.

### Levantamento e análise de requisitos:
Compreender as necessidades do usuário e o que o usuário deseja que o sistema realize. Um sistema bem modelado depende de um levantamento de requisitos bem validado com o usuário.

### Blocos de construção da UML:
#### Itens:
- Itens estruturais (estáticos): São partes estruturais do modelo, existem antes de qualquer ação acontecer. Representam elementos conceituais (entidades do modelo conceitual) e físicos (no modelo físico) (classes, colaborações, casos de usos...). Ex: classes como Cliente, Produto...;
- Itens comportamentais (Dinâmicos): São ações e movimentos durante o funcionamento do sistema que mudam o estado de algo. Ex: Depositar, AuemntarCrédito...;
- Itens de agrupamento (Pacotes): São diretórios organizacionais da UML. Blocos onde os modelos podem ser organizados de acordo com seu nicho;
- Itens anotacionais (Notas): São as partes explicativas do modelo na UML (comentários e observações). Ex: pequenos textos anexados no desenho lembrando uma regra importante.

#### Relacionamentos:
- Relacionamento de associação: Relacionamento estrutural entre classes que descreve um conjunto de ligações em que, as ligações são conexões entre objetos que são instâncias das classes;
- Relacionamento de generalização: É um relacionamento de especialização/generalização no qual os objetos dos elementos especializados (filhos) são substituídos por objetos do elemento generalizado (pais). Assim, os filhos compartilham a estrutura e o comportamento dos pais (**herança da POO**).
- Relacionamento de dependência: É um relacionamento semântico entre dois itens onde a alteração do item independente altera a semântica do item dependente;
- Relacionamento de realização: É um relacionamento especial que mistura características dos relacionamentos de generalização e dependência. Utilizada no diagrama por identificar classes que exercem funções para as classes que representam interfaces.
---
## DIAGRAMAS

### Diagramas de casos de uso:
  - **Onde se descreve o que o usuário quer e como deve ser feito;**
  - Representa os cenários identificados e coletados dos usuários;
  - Possibilita a compreensão do comportamento do sistema por qualquer pessoa (interação com o usuário, comportamento externo e interno);
  - Empregado no início da modelagem (levantamento de requisitos);
  - Guia para modelagem de outros diagramas.
  - Deve captar o comportamento do sistema por meio da análise de requisitos;
  - Pode adotar recursos gráficos para melhor interpretação dos requisitos;
  - Permite documentar todos os requisitos,
  - Estrutura simples e linguagem natural informal, fácil interpretação de todos os envolvidos (stakeholders);
  - Organiza requisitos e eliminar redundâncias;
  - Identifica possíveis riscos para a fase de construção do sistemas;
  - Possibilidade de ser empregado em qualquer uma das fases do desenvolvimento do sistema.
  
### Ator:
Papéis desempenhados por qualquer usuário de um caso de uso. O ator é quem solicita os serviços disponíveis em casos de uso.
  - Uma pessoa que interage com o sistema;
  - Um hardware que interage com o sistema;
  - Um outro sistema com a necessidade de utilizar o caso de uso.

**Perguntas para identificar atores:*** 
  - Quem utiliza a funcionalidade principal (Atores principais)?
  - Quem irá manter, administrar e manter o sistema operante?
  - Quem proverá suporte ao sistema em seu processamento diário?
  - Quem/O quê tem interesse nos resultados produzidos pelo sistema?
  - Com quais outros sistemas o sistema em foco irá interagir?

### Casos de uso:
Serviços, tarefas ou funções que são utilizados pelos usuários (atores) do sistema. Ex: CadastrarCliente, VerificarCadastroCliente...

### Documentação dos casos de uso:
Notação diagramática - diagrama de caso de uso da UML;

Notação textual - descrição dos casos de uso (Não há notação especifica para a textual, varia de criador a criador).

#### Casos de uso textuais:
Mostrar a sequência típica de eventos (cenários de sucessos principais) e as sequências alternativas que podem ocorrer durante o caso de uso. Mostrar interessados e interesses do caso de uso.
ex:
  
  Digita login correto -> Digita senha correta -> Entra no servidor;
  
  Digita login errado -> Digita senha correta -> Erro de login. Login inválido
...
FIM DA AULA, SLIDE 32
