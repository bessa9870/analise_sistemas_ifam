# O COMPONENTE HUMANO NO DESENVOLVIMENTO DE SOFTWARE
*11-08-26 | Análise de sistemas*

O desenvolvimento de um software complexo é feito em equipe. Vejamos alguns dos componentes:
###**Gerente de projeto**
  - Gerencia, coordena e monitora a equipe;
  - Controle de orçamento de tempo, recursos e gastos do projeto;
  - Definição dos programas e processos de desenvolvimento(software/hardware, frameworks, banco de dados...);
  - Suprir as necessidades do cliente(usuário), fazer o programa ser necessário;
  - Só deve haver um gerente por projeto.

###**Analista**
  - Conhecimento do domínio do negócio do cliente (fazer o dever de casa sobre o negócio do cliente);
  - Capacidade de comunica-se com os especialistas do domínio do negócio (aprender os vocabulários);
  - Traduzir os requisitos do cliente ao sistema e a equipe;
  - Domínio da programação e aprendizado rápido;
  - Ética e fácil comunicação com pessoas de todos os tipos.

###**Projetista**
  - Avalia e propõe a melhor alternativa para o sistema físico;
  - Propõe soluções para problemas encontrados nas análises;
  - Gera especificações para soluções computacionais detalhadas.
  - Especialidades:
    - Interface;
    - Banco de dados;
    - Redes e segurança. 

###**Arquiteto de software**
  - Elabora a arquitetura de todo o sistema(interfaces);
  - Toma decisões globais sobre detalhes técnicos(performance, confiabilidade e codificação);
  - Conhecimento sobre o domínio do negócio do cliente;
  - Gerente técnico do sistema;

###**Programador**
  - Escreve os códigos, alta habilidade em programação;
  - Interpretação e transcrição de diagramas e documentação para linhas de código;
  - Rapidez na construção do código;
  - Controle de versionamento e conhecimento das tecnologias modernas;
  - Entender o que, porque e como está implementando.

###**Clientes**
  - A pessoa com a necessidade do sistema. Existem dois tipos de cliente:
      - Cliente usuário: Entende do negócio, fará uso do sistema efetivamente, entende da necessidade;
      - Cliente contratante: Chamado executivo patrocinador, é quem contrata e paga pelo sistema.

*Independente do processo de desenvolvimento, o envolvimento e comprometimento do usuário final na construção do sistema é indispensável.*

###**Avaliadores da qualidade (QA)**
  - Realizam testes de conformidade, validação, desempenho, confiabilidade...
  - Escrevem manuais a partir da documentação;
  - Garante a qualidade.

---
# MODELOS DE CICLO DE VIDA

As atividades para o desenvolvimento de sistemas são idênticas, existem duas grandes categorias:
  - Modelo em cascata
  - Modelo interativo e incremental

## Ciclo de vida de modelo em cascata 
É o modelo linear/clássico, progressão sequencial de uma classe a outra. Eventual retroalimentação de uma fase a outra.
  - Problema 1: Processos reais não são sequenciais, podendo haver atividades paralelas;
  - Problema 2: Não é possível reunir todos os requisitos na fase de levantamento;
  - Problema 3: Leva muito tempo para o usuário interagir com o sistema e verificar se suas expectativas estão sendo atendidas (a versão de produção é a última fase) a velocidade das mudanças, concorrência das organizações no mercado e a complexidade torna esse modelo de ciclo de vida obsoleto e inútil.

## Ciclo de vida de modelo iterativo incremental
Desenvolvimento em ciclos, em cada ciclo são levantados requisitos e executadas atividades de análise, projeto, implementação e testes. Para cada ciclo se estabelece uma meta que deve ser atingida. Os ciclos se repetem até que todos os requisitos sejam implementados.
  - Deve haver mecanismo de agrupamento e divisão de requisitos por prioridade;
  - Iterativo porque o sistema é desenvolvido em passos similares, é incremental em cada volta são adicionadas novas funcionalidades ao sistema e correção de erros.
  - 
Incentiva a participação(interação via teste de sistema), porém é mais complexo de se gerenciar, suas atividades são executadas repetidamente e em paralelo, equipes trabalham em vários requisitos simultaneamente.

Possui melhor gerenciamento de riscos de desenvolvimento, para evitar:
  - São satisfazer requisições;
  - Falta de verba/orçamento;
  - Software não adaptável;
  - Fatores externos.

Os requisitos mais nocivos devem ser atendidos primeiro. As inconsistências devem ser identificadas em cada ciclo e extinguidas no ciclo seguinte, mas pode haver (no pior caso) um único ciclo apenas para extinguir inconsistências(não deixar inconsistências se acumulares).

O processo de desenvolvimento iterativo incremental é dividido em duas fases: Tempo(fase) e Atividades.
  - Tempo: Atividades que podem ser cumpridas por uma ou mais iterações que resultam em incrementos;
  - Atividades: Ações como levantamento de requisitos, projeto, implementações, testes e implantação.

### Fases:
  - Concepção: Ideia geral e escopo. Planejamento de alto nível e estabelecimento de marco;
  - Elaboração: Como será implementado, projeto de desenvolvimento completo, análise do domínio do negócio, requisitos priorizados, iterações, seus próximos incrementos e durações da próxima fase definidas.
  - Construção: Muitas análises e projetos. muitas iterações até o sistema poder ser entregue ao usuário, elaboração dos manuais e documento final de consulta e referência.

*As iterações devem ser feitas principalmente na fase de construção, mas é possível tê-las nas demais fases.*

## Utilização da UML no processo iterativo incremental
Ferramenta independente que produz artefatos que serão lidos pelo programador que os adicionará no sistema. A cada iteração, novos detalhes devem ser adicionados. A construção de um artefato fornece os detalhes que devem ser adicionados a outros artefatos em um esquema de iteração contínua para capturar todos os requisitos do sistema.

## Prototipagem
  - **Técnica usada quando o entendimento das requisições é difícil**
  - Técnica que completa a análise de requisitos;
  - Usar protótipos para telas(entradas/saídas), subsistemas ou o sistema como um todo;
  - O usuário é quem valida o protótipo. Usado quando o entendimento de requisitos é difícil;
  - Tornam a validação menos arriscada(o cliente vê o que vai receber);
  - Não devem substituir diagramas e nem virar o sistema.

*Pode utilizar programas de representações gráficas ou linguagens de programação*

## Ferramentas de suporte ao processo de desenvolvimento

*CASE - Computer Aided Software Engeneering*
  - Criação de diagramas e manutenção consistência entre eles;
  - Round-trip engeneering: geração de códigos via diagrama e vise versa
  - Depuração de código-fonte: Encontrar erros de lógica na estrutura;
  - Realizar testes automaticamente no sistema;
  - Controle de versionamento: gerencia versões dos artefatos/códigos-fonte durante o ciclo de vida;
  - Verificação de desempenho: Averigua o tempo de execução de módulos e tráfego de dados na rede;
  - Verificação de erros em tempo real;
  - Gerenciamento de mudanças de requisitos. 
