## Caso de Uso 01: Realizar Empréstimo de Livro:
  - Ator: Associado, Bibliotecário (ou Sistema).
  - Pré-condições: O associado deve estar cadastrado e o sistema deve ter exemplares disponíveis do livro desejado.
  - Pós-condições: O empréstimo é registrado no histórico do associado e os exemplares são marcados como indisponíveis no acervo.
  - **Fluxo principal:**
  1. O associado solicita o empréstimo de exemplares.
  2. O sistema verifica a quantidade atual de livros já emprestados ao associado.
  3. O sistema confirma que o associado possui menos de 3 exemplares emprestados.
  4. O sistema registra a data atual para o novo empréstimo.
  5. O sistema vincula o(s) exemplar(es) ao código do associado.
  6. O sistema confirma o empréstimo.
  -  **Fluxo de Exceção (Limite Excedido):**
  -  No passo 3, se o associado já tiver 3 livros emprestados, o sistema exibe uma mensagem de erro informando que o limite máximo foi atingido e cancela a operação.
  
## Caso de Uso 02: Realizar Devolução de Livro
