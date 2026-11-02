 # Revisão de times e permissões no GitHub

## Pasta `.github`

A pasta `.github` reúne arquivos de configuração e colaboração do repositório, como modelos de issues e pull requests, fluxos de trabalho e documentação. Este arquivo, `revisao-teams.md`, registra orientações para revisar os times e as permissões de uma organização. Consulte o conteúdo atual da pasta antes de inventariar seus arquivos; não presuma a existência de arquivos que não estejam presentes.

## Objetivo da revisão

Verificar se os times da organização representam grupos de trabalho atuais, têm responsáveis definidos e recebem apenas o acesso necessário. A revisão deve considerar tanto as permissões do time na organização quanto o acesso concedido a cada repositório.

## Times e associação

- Confirme o propósito, os responsáveis e os repositórios associados a cada time.
- Revise a lista de integrantes e remova acessos de pessoas que não precisem mais deles.
- Prefira conceder acesso por meio de times, em vez de atribuí-lo individualmente, sempre que isso atender à necessidade.
- Verifique times aninhados, quando usados, e considere que o acesso pode ser herdado pelos times subordinados.
- Use nomes e descrições que deixem claro a finalidade do time.

## Níveis de acesso a repositórios

As permissões disponíveis podem variar conforme o tipo de repositório e as políticas da organização. Em geral, os níveis comuns são:

| Permissão | Uso geral |
| --- | --- |
| `Read` | Consultar e clonar o repositório; adequada para quem precisa apenas acompanhar o projeto. |
| `Triage` | Gerenciar issues e pull requests sem permissão para enviar alterações ao código. |
| `Write` | Enviar alterações e colaborar em issues e pull requests. |
| `Maintain` | Administrar aspectos do repositório sem controle total sobre configurações sensíveis. |
| `Admin` | Controle amplo do repositório, incluindo configurações e acesso; reservar a responsáveis que realmente necessitem desse nível. |

Conceda a permissão mínima necessária para cada atividade. Não confunda as permissões de um repositório (`Read`, `Triage`, `Write`, `Maintain` e `Admin`) com funções da organização, como proprietário (`Owner`) ou integrante (`Member`): são escopos diferentes. Permissões adicionais, como acesso a pacotes ou recursos específicos, devem ser revisadas separadamente.

## Checklist de revisão

- [ ] Relacionar os times existentes, seus objetivos e responsáveis.
- [ ] Confirmar integrantes e remover associações obsoletas.
- [ ] Revisar os repositórios vinculados a cada time.
- [ ] Conferir se cada permissão corresponde à necessidade atual, reduzindo acessos excessivos.
- [ ] Revisar concessões diretas a pessoas e acessos herdados por times aninhados.
- [ ] Confirmar se os acessos administrativos estão limitados e justificados.
- [ ] Registrar alterações, justificativas, responsável pela revisão e data.
- [ ] Revisar novamente após mudanças de equipe, projeto ou necessidade de acesso.

## Registro

| Data | Revisor(a) | Times/repositórios revisados | Alterações e justificativas |
| --- | --- | --- | --- |
|  |  |  |  |
