## Criando um Branch
### Para começar a trabalhar com branches, o primeiro passo é criar um branch no repositório local. Isso pode ser feito com o comando:
```bash
git branch <nome-do-branch>
```

- **Este comando cria um novo branch baseado na revisão atual**. Se você quiser criar o branch a partir de uma revisão específica, pode fornecer o hash SHA-1 correspondente:

```bash
git branch <nome-do-branch> <hash-da-revisao>
```

## Renomeando um Branch
- Se precisar corrigir um nome de branch ou simplesmente renomeá-lo, você pode usar o seguinte comando:
```bash
git branch -m <novo-nome>
```

- Para renomear um branch que não esteja atualmente ativo, forneça o nome antigo e o novo:
```bash
git branch -m <nome-antigo> <novo-nome>
```
Renomear branches remotos requer um processo diferente, envolvendo a exclusão do branch antigo e o push do novo branch.

## Alternando Entre Branches
- Alternar entre branches é uma das operações mais comuns. Isso pode ser feito com:

```bash
git checkout <nome-do-branch>
```

**Ou, para uma abordagem mais clara, você pode usar o comando switch:**
```bash
git switch <nome-do-branch>
```

Publicando um Branch
Depois de criar um branch local, você pode publicá-lo em um repositório remoto usando:
```bash
git push -u origin <nome-do-branch> 
```
- **o (-u) seta o upstream para as proximas vezes rodar apenas o comando principal, isso funcionando mudando de branch ou enviando**
- Este comando também estabelece uma conexão de rastreamento, facilitando futuros pushes e pulls.

## Deletando um Branch
Branches que não são mais necessários podem ser deletados com o comando:
```bash
git branch -d <nome-do-branch>
```
Como deletar branch remota no Git de forma automatizada: https://devopsmind.com.br/shell-script-pt-br/deletar-branch-remota-git/

- Para deletar um branch remoto, use:
```bash
git push origin --delete <nome-do-branch>
```

## Fazendo Merge de Branches
O merge é usado para integrar as mudanças de um branch ao branch principal. Para isso:
```bash
git switch main
git merge <nome-do-branch>
```
Isso cria um commit de merge, combinando as alterações dos dois branches.

## Revisao de arquivos
#### Além desses comandos tem revisões de arquivos por Dots (..) & (...)
- Comparação definitiva: .. vs. ...
**Comando	Significado**
```bash
git log main..feature-a	Commits presentes em feature-a, mas não em main.
git log main...feature-a	Commits exclusivos de qualquer uma das duas branches.
git diff main..feature-a	Compara os estados dos arquivos das duas referências.
git diff main...feature-a	Compara a versão de feature-a com o ponto de divergência entre as branches.
```

