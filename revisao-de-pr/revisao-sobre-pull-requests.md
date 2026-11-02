# Revisão sobre pull requests

Um **pull request (PR)** propõe alterações para revisão antes de incorporá-las a uma branch. Uma **issue** registra uma tarefa, um problema ou uma melhoria. Relacionar os dois facilita acompanhar o trabalho e entender quais mudanças atendem a cada demanda.

## Como relacionar um pull request a uma issue

Na descrição do PR, mencione a issue usando `#` seguido do número, como `#42`. Para que ela seja fechada automaticamente quando o PR for integrado à branch padrão, use uma palavra-chave:

- `Closes #42`
- `Fixes #42`
- `Resolves #42`

Essas palavras-chave também podem ser usadas em uma mensagem de commit associada ao PR.

## Como relacionar uma issue a um pull request

Mencione o número do PR em um comentário ou na descrição da issue, por exemplo: “Implementação proposta em #57”. Também é possível usar a seção **Development** da issue para vincular o PR correspondente.

Em resumo, a issue descreve **o que precisa ser feito**, enquanto o PR apresenta **as alterações propostas**. Manter ambos vinculados deixa o acompanhamento, a revisão e o histórico do trabalho mais claros.