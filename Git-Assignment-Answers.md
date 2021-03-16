# Git Assignment

**Aluno: Lucas Vinicius Ribeiro**


**Entrega**: 16-Mar-21

## Como entregar
Copie o arquivo em seu repositorio e coloque as respostas nas caixas
Abra uma issue nesse repositório aqui indicando o link para o arquivo no seu repo.

### Entenda o repositorio
Para fazer isso, você terá que baixar [handson.zip] (handson.zip) e descompactá-lo.
A pasta handson é um repositório git. Usando a linha de comando, altere o diretório para "handson /"

As caixas vazias
```

```
representam o conteúdo que você precisa preencher e postar em seu repositório privado

1. Descreva qual é a saída dos seguintes comandos
    -  `git branch` 
    -  `git checkout BRANCH_NAME` (USE THE NAME OF AN EXISTING BRANCH)
    -  `git log --decorate`

```
    -  `git branch`: Lista as branches existentes no repositório e destaca a branch atual.
    -  `git checkout BRANCH_NAME`: Troca para a branch desejada.
    -  `git log --decorate`: Mostra a lista de commits e suas informações básicas (ID, Autor, Data, Mensagem) e também mostra para qual branch o HEAD está apontando.

```

2. Tente usar `git log --graph --all`. O que acontece?
```
Exibe graficamente o histórico de commits de todas as branches existentes no repositório.

```

3. Use `git diff BRANCH_NAME`  para ver as diferenças de um ramo e do ramo atual.
   Sumarize as diferenças do master e do outro ramo.

```
No arquivo A.java, a branch feature-foo possui o método foo(), enquanto na branch master esse método não existe.
No arquivo B.java, a branch master possui a definição da classe B, enquanto na branch feature-foo o arquivo está vazio.

```

4. Escreva uma sequencia de comandos para mesclar o ramo não-master no `master`

```
`git merge feature-foo`

```


5. Escreva um comando (ou sequência) para (i) criar um novo ramo chamado `math` (do` master`)
e (ii) mudar para este ramo

```
`git branch math`
`git checkout math`

```
   
6. Edite B.java adicionando o código abaixo ao conteúdo do arquivo
```java
System.out.println("I know math, look:")
System.out.println(2+2)
```

7. Escreva o comando (ou sequencia) para realizar o commit de suas mudanças
```
`git commit -a -m "Print math operations"`

```

8. Volte para o branch `master` e mude B.java adicionando o seguinte código-fonte (confirme sua mudança para` master`):
```java
System.out.println("Hello World")
```

9. Escreva uma sequência de comando para mesclar o branch `math` em` master` e descreva o que aconteceu
```
Deu conflito entre as alterações realizadas em branches distintas, no mesmo arquivo (B.java).

```
   
10. Escreva um conjunto de comandos para abortar a mesclagem
```
`git merge --abort`

```
   
11. Agora repita o item 9, mas prossiga com a mesclagem manual (Editando B.java). Todas as funções implementadas são necessárias. Explique o seu procedimento
```
Após a execução do comando `git merge math`, editei manualmente o arquivo B.java, removendo as marcações adicionadas pelo git, mantendo as alterações realizadas em ambos os commits.

```

12. Escreva um comando (ou conjunto de comandos) para prosseguir com a mesclagem e atualizar o branch `master`
```
`git commit -a -m "Fixed conflicts"`

```


