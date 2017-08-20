# Git (exercícios)


#### 1. Qual o comando para obter a versão instalada do Git?
<pre>git version</pre>

#### 2. Qual o efeito da execução de cada um dos comandos abaixo?  

- git config -l 
<pre>Escreverá a partir do arquivo especificamente.</pre>  

- git mv a.txt b.txt 
<pre>Renomea o arquivo</pre>

- git reset –hard 
<pre>Retorna a copia de trabalho para o conteúdo do repositório (HEAD) Todo o conteúdo do repositório. 
Arquivos criados e não adicionados não são removidos</pre>

- git log -27 
<pre>Fornece os logs dos commits até o de número 27</pre>

- git help 
<pre>Disponibiliza o manual de ajuda para qualquer comando do git</pre>

- git help reset 
<pre>Se obtem ajuda especifica para o comando reset.</pre>

- git add –all 
<pre>Prepara todos (--all) os seus arquivos para o commit</pre>

- git add -u 
<pre>Adiciona todos os arquivos modificados que já são monitorados pelo git</pre>


#### 3. O fluxo “clássico” de interação com o Git é algo como “realizar trabalho em um ou mais arquivos e diretórios”, “acrescentá-los para serem contemplados” e, finalmente, executar um “commit”. Quais os comandos necessários para realizar os dois últimos “passos” desse fluxo?
<pre>
git add <nome>
git add -u
git commit -m “comentário”
git push
     </pre>

#### 4. Qual o comando deve ser executado para identificar o que foi alterado desde o último “commit”?
<pre>gti show commit </pre>

#### 5. Em um dado repositório, arquivos simplesmente copiados para lá, ou seja, untracked, podem ser exibidos/identificados com que comando?
<pre>git status</pre>

#### 6. Qual o comando para efetuar um commit?
<pre>git push</pre>

#### 7. Qual o comando que devemos empregar para descartar mudanças ocorridas no arquivo teste.txt, por exemplo?
<pre>git checkout teste.txt</pre>

#### 8. O que deve ser feito para que um determinado diretório do seu repositório seja ignorado pelo Git?
<pre>Fazer um arquivo chamado .gitignore e dentro do arquivo digita o nome ou endereço da pasta que se quer ignora.</pre>

#### 9. O que acontece se o seu repositório local for removido?
<pre>A exclusão de um repositório privado irá apagar todos os seus garfos.
A exclusão de um repositório público não vai apagar os seus garfos.</pre>

#### 10. Como clonar um repositório remoto?
<pre>git clone <URL>.git</pre>

#### 11. Em alguns cenários git log pode produzir extensos resultados. Se houver interesse em visualizar o histórico de um repositório, onde cada mudança é fornecida exatamente em uma única linha, qual o comando que deve ser empregado?
<pre>git shortlog -sne</pre>

#### 12. Em qual arquivo o Git armazena informações de configuração empregadas por usuário?
<pre>Arquivo .gitconf</pre>

#### 13. Qual o comando para criar um repositório local?
<pre>git init</pre>

#### 14. Qual o nome do diretório criado pelo Git quando se executa o comando git init?
<pre>origin</pre>

#### 15. Qual o comando para adicionar todos os arquivos modificados? (Aqueles para os quais git status identificam como modified?)
<pre>git add -u</pre>

#### 16. O Git faz uso do valor de hash conhecido por SHA1. O que isto significa? Qual o propósito? O que é SHA1?
<pre>É a chave de identificação de cada commit, usado para especifica-lo na hora de usar alguns comandos</pre>

#### 17. Qual a palavra para indicar o último commit em vez do valor de hash SHA1 correspondente?
<pre>HEAD~1</pre>

#### 18. Quando se cria dois arquivos usando um editor de texto qualquer e, na sequência, executamos o comando git add -u, os dois arquivos criados passam de untracked para new file?
<pre>Sim</pre>

#### 19. Qual o efeito da execução dos dois comandos abaixo, nesta ordem, em um dado repositório?
<pre>git reset --soft HEAD~1 Se desfazer do último commit
git reset –hard Retorna a copia de trabalho para o conteúdo do repositório (HEAD). 
Exeto do ultimo commit por foi utilizado git reset --soft HEAD~1.</pre>

#### 20. Após o emprego de um ambiente integrado de desenvolvimento (IDE), é comum a criação de arquivos e diretórios. Qual o comando que podemos empregar para remover arquivos e diretórios untracked?
<pre>git clean -f</pre>

#### 21. Qual o nome do arquivo no qual podemos inserir a indicação para o Git de arquivos e diretórios a serem ignorados?
<pre>git checkout --"arquivo" </pre>

#### 22. Quando se cria o arquivo MinhaClasse.class em um dado diretório e desejamos que o Git ignore não apenas este, mas arquivos .class em geral, por todos os membros de uma equipe que estão contribuindo com um dado projeto?
<pre>git reset HEAD</pre>

#### 23. jQuery é uma famose biblioteca em JavaScript. Consulte detalhes em http://jquery.com. O repositório Git correspondente encontra-se disponível em https://github.com/jquery/jquery.git. Faça o clone deste repositório jqueryrepo.
<pre>Feito</pre>

#### 24. No repositório jqueryrepo, criado no passo anterior, qual o efeito do comando git shortlog -sne?
<pre>Apresenta histórico do repositório</pre>

#### 25. No repositório jqueryrepo, qual o efeito de git remote -v?
<pre>Exibe o nome e a URL do repositório</pre>

#### 26. Um repositório Git pode ser etiquetado ao longo do tempo. Ou seja, commits específicos podem ser “marcados” ou “etiquetados” para facilitar referências posteriores. Para listar todas as “etiquetas” (tags) estabelecidas para um dado repositório, qual comando deve ser executado?
<pre>git merge "branchNome" </pre>

#### 27. Caso um dato repositório retorne muitas “marcas” ou “etiquetas” para o comando git tag, como retornar apenas aquelas que atendem a determinado padrão, por exemplo, iniciadas por 2.0?
<pre>git tag -a 2.0</pre>

#### 28. Qual o efeito do comando git tag -a 3.4-gold -m “minha versão ouro”?
<pre>Too many params</pre>

#### 29. Após executado o comando acima, qual o efeito de git show 3.4-gold?
<pre>Exibe as diferenças introduzidas no repositório pelo ultimo commit</pre>

#### 30. O que o comando git push origin 3.4-gold teria como efeito?
<pre>O git coloca os commit no repositório 3.4-gold</pre>

#### 31. Após executar um commit, qual o efeito de git commit –amend?
<pre>Refaz commit quando esquecer de adicionar um arquivo no Stage >> 
O amend é destrutivo e só deve ser utilizado antes do commit ter sido enviado ao servidor remoto</pre>

#### 32. Após executar git add x.txt, qual o efeito de git reset HEAD x.txt?
<pre>Remove arquivos versionados e modificados do Stage</pre>

#### 33. Após alterar o conteúdo de um arquivo committed em passo anterior, qual o efeito do comando git checkout – a.txt?
<pre>Desfaz modificações de arquivos versionados no Stage</pre>

#### 34. Qual a diferença entre os comandos git reset HEAD x.txt e git checkout -- a.txt?
<pre>O git reset HEAD x.txt remove arquivos versionados e modificados do Stage e 
o git checkout -- a.txt desfaz modificações de arquivos versionados no Stage</pre>
