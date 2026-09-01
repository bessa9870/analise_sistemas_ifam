# Aula 2 | Análise de sistemas | 04-08-26 

## Evolução histórica

  1950 - 1960: Fluxograma e diagramas
  1970: Programação estruturada 
  1990: Análise orientada à objetos

## A Linguagem de modelagem unificada (UML)

  James Ramboaugh(OMT) Grady Booch e Ivar Jacobson(DOSE) propuseram a UML apovada em 1997 pela OMG. UML é uma linguagem visual que representa os conceitos 
da programação orientada à objetos em várias pespectivas de sistema onde cada elemento possui sintaxe. Os autores da UML sugerem 5 visões:
  Visões de casos de uso: Como o usuário trabalha, na scrum é a história de usuário, como o sistema deve interagi com o mundo exterior(principal);
  Visões de projeto: Características estruturais e comportamentos externos e internos;
  Visões de implementação: Distribuição e implantação das formas físicas do sistema
  Visão de implantação: Fluxo de execução do sistema;
  Visão de processo: Sincronização, concorência e desempenho do sistema;

## Processo de desenvolvimento de software(PDS)

  É uma atividade complexa que corresponde a sobreposição das complexidades relativas ao desenvolvimento dos seus diversos componentes: Software, hardware,
procedimento, comunicação e pessoas. Esse processo deve minimizar problemas e garantir a qualidade, ele deve incluir todas as atividades necessárias para:
Definir o que deve ser feito, desenvoler, testar e manter. Entre seus objetivos: Como, quando e por quem as atividades serão executadas, pontos de controle 
para verificar o andamento do projeto(padronizar o processo de desenvolvimento do software).
  Processos de desenvolvimento previstos:
  Levantamento de requisitos: Desenvolvedores e clientes tentam criar a mesma visão da solução a ser construída (ex: um dev e um vendedor de óculos);
  Requisito: Capacidade/exigência/necessiade a ser alcançada para satisfazer documentos formalmente impostos(Maciasszek 2000);

## Atividades típicas de um processo de desenvolvimento de software

  Requisitos estão circunscritos ao domínio do negócio(parete relevante da realidade que é relevante para a constução do sistema). Fase de estudo exploratório
do negócio do cliente, fontes:
  Necessidades atuais;
  Sistema atual(se existir);
  Leitura de referências e documentos;
  Observação do ambiente;
  Entrevista com usuários e especialistas de domínio de negócio(especialista no negócio do cliente);
  Reutilização de análises anteriores;
  Comparação com outros sistemas do mesmo domínio.

## DOCUMENTO DE REQUISITOS

  O produto dessa atividade é o DOCUMENTO DE REQUISITOS escrito emn notação informal contendo: 
  Requisitos funcionais: parte dinâmica, funcionalidades do sistema e requisitos não-funcionais;
  Confiabilidade: Tempo médio entre falhas, recuperação de falhas, quantidade de erros...;
  Desempenho: Tempo de resposta e otimização para funcionalidades;
  Portanilidade: 
  Restrições: Delimita o programa aos custos e prazos, plataformas, tecnologias aspectos legais e etc.

  A qualidade, sucesso e utilidade de um sistema é medida pelo grau de atendimento aos requisitos, o usuário deve tornar-se dependente do sistema. Os requisitos
devem atender leitores técnicos(para demais necessidades de soluçĩoes técnicas) e uusarios(para saber como manusear). O documento de requisitos deve responder a
pergunta "o que o usuário necessita do novo sistema?", sistemas são avaliados pelo grau de conformidade e definem o problema a ser resolvido pelo sistema independente
da tecnologia usuada. 

  O levantamento de requisitos ao cliente é a etapa mais importante no retorno de investimentos feitos no projeto pelos desenvolvedores, o desenvolvedor deve compreender 
bem os processos antes do início do desenvolvimento para apresentá-lo ao cliente. O levantamento deve servir para se compreender o sistema o máximo o possível. 

  O documento de requisitos deve ser o consenso entre cliente e desenvolvedor levando em consideração a possível volatilidade dos requisitos(expectativas dos usuários, 
tecnlogias utilizadas, mercado e etc).

  Ao quebrar o levamentamento de requisitos, entender como os componentes interagem e capturar seu funcionamento, detalha-se a construção de modelos.
  Validação e verificação.
  Só quem pode garantir a validação e o verificação dos modelos, os modelos devem representar as classes de objetos e funcionalidades do sisema.
  Projeto: Determina como o sistema vai funcionar, as restrições tecnológicas e arquitetura do sistema.

  Implementação: Construção o código.
