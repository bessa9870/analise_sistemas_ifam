## Caso de uso 01 - Cadastrar livro:
  - Ator: Bibliotecário / Sistema.
  - Pré-condições: O ator deve estar cadastrado e validado no sistema. O ator deve estar com o livro e exemplares junto das informações preparadas para ser registrado no banco.
  - Pós-condições: O livro e exemplares devem estar preparados para movimentação imediatamente após o processo de registro.

**Fluxo principal:**
  1. O ator registra as informações do livro, título, autor/autores, gênero e ISBN.
  2. O ator registra as palavras-chaves que descrevem aquele livro. 
  3. Seguidamente, o ator informa ao sistema o número de exemplares (se houver).
  4. O ator confirma o registro das informações do livro no sistema.
  5. O ator aloca os exemplares nas prateleiras do gênero registrado no sistema.

## Caso de Uso 02 - Realizar Empréstimo de Livro:
  - Ator: Associado, Bibliotecário / Sistema.
  - Pré-condições: O associado deve estar cadastrado e o sistema deve ter exemplares disponíveis do livro desejado.
  - Pós-condições: O empréstimo é registrado no histórico do associado e os exemplares são marcados como indisponíveis no acervo.

**Fluxo principal:**
  1. O associado solicita o empréstimo de exemplares.
  2. O sistema verifica a quantidade atual de livros já emprestados ao associado.
  3. O sistema confirma que o associado possui menos de 3 exemplares emprestados.
  4. O sistema registra a data atual para o novo empréstimo.
  5. O sistema vincula o(s) exemplar(es) ao código do associado.
  6. O sistema confirma o empréstimo.

**Fluxo de Exceção (Limite Excedido):**
  -  No passo 3, se o associado já tiver 3 livros emprestados, o sistema exibe uma mensagem de erro informando que o limite máximo foi atingido e cancela a operação.
  
## Caso de Uso 03 - Realizar Devolução de Livro
  - Ator: Bibliotecário / Sistema.
  - Pré-condições: O exemplar entregue deve constar como "emprestado" no histórico do associado.
  - Pós-condições: O exemplar retorna ao acervo, a data de devolução é registrada e um recibo é gerado.
  
**Fluxo Principal (Devolução no Prazo):**
  1. O bibliotecário insere os dados do exemplar devolvido no sistema.
  2. O sistema localiza o empréstimo no histórico do associado.
  3. O sistema calcula o tempo de empréstimo (diferença entre data atual e data de empréstimo).
  4. O sistema constata que o tempo é igual ou inferior a uma semana.
  5. O sistema registra a devolução e altera o status do exemplar para disponível.
  6. O sistema gera e imprime o recibo de entrega do livro.

**Fluxo Alternativo (Devolução com Atraso):**
  1. No passo 4, se o tempo de empréstimo for superior a uma semana:
  2. O sistema calcula a multa (R$ 2,00 multiplicados pelo número de dias de atraso).
  3. O sistema informa o valor detalhado da multa na tela antes da impressão.
  4. O bibliotecário confirma a visualização.
  5. O sistema gera e imprime o recibo de entrega contendo o detalhamento da multa.

## Caso de Uso 04 - Registrar Extravio e Reposição de Livro
  -  Ator: Associado, Bibliotecário.
  -  Pré-condições: O exemplar deve estar atualmente emprestado ao associado que relata o extravio.
  -  Pós-condições: A pendência do exemplar é resolvida e um recibo específico é anexado ao histórico do associado.
  
**Fluxo Principal:**
  1. O associado informa o extravio do exemplar ao bibliotecário.
  2. O sistema localiza o registro do empréstimo ativo.
  3. O bibliotecário seleciona a opção de extravio no sistema.
  4. O sistema apresenta as opções de: reposição do mesmo livro ou pagamento do valor de um exemplar novo.
  5. O associado escolhe uma das opções e realiza a entrega do novo livro ou o pagamento.
  6. O sistema registra a opção escolhida.
  7. O sistema gera um documento de recibo específico de extravio/reposição.
  8. O sistema salva este recibo no histórico permanente do associado.

## Caso de Uso 05 - Gerar Relatório de Movimentação 
  - Ator: Bibliotecário / Sistema
  - Pré-condições: O sistema deve conter dados registrados de associados e histórico de empréstimos.
  - Pós-condições: Um relatório consolidado é exibido ou impresso.
  
**Fluxo Principal:**
  1. O ator solicita a emissão do relatório de fechamento de período.
  2. O ator insere o período desejado para coletar os dados.
  3. O sistema varre o banco de dados e lista de todos os livros emprestados no período solicitado.
  4. O sistema contabiliza o número total de associados cadastrados no período solicitado.
  5. O sistema formata os dados e gera o documento final do relatório.
