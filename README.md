# Relatório Parcial 1

Baseado no PFC (Projeto Final de Curso) aka TCC (Trabalho de Conclusão de Curso) dos
alunos Jan Segre e Victor Bramigk do IME (Instituto Militar de Engenharia).
https://www.github.com/roboime/pfc-jan-bramigk/

## Requisitos

`sudo apt-get install texlive-latex-base`

`sudo apt-get install texlive-latex-extra`

`sudo apt-get install latex2html`

Para obter o arquivo abntex2.cls:

`sudo apt-get install texlive-publishers`

Para instalar o pacote brazil.ldf:

`sudo apt-get install texlive-lang-portuguese`

Para instalar o pacote algorithm2e.sty:

`sudo apt-get install texlive-science`

Instalar o pygmentize, para o pacote minted funcionar,
baixei o código fonte em:
https://pypi.python.org/pypi/Pygments#downloads

Conferir se as linhas 156-218 estão comentadas

linha 84 de CMakeLists.txt precisa ter '_consideracoes.tex' em vez de 'cons_finais.tex'

Após as dependências estarem construídas, digitar os comandos:

`cd "pasta do projeto"`

`mkdir build`

`cd build`

`cmake .. && make pdf`

## Como adaptar o projeto

Criar os documentos preferencialmente na pasta `/doc`

Copiar os modelos de `doc/modelagem.tex` para capítulos e de `doc/ssl.tex` para seções

alterar os "cabeçalhos" dos arquivos, substituir texto

Inserí-los no texto com o comando `\input{doc/nome_sem_extensao}`

Lembrar de adicioná-los em CMakeLists.txt, na seção DOC (IMG para imagens)

Observar comentários com `@PÍCOLI` ou `PÍCOLI`, há varias coisas que já foram implementadas no projeto original (pfc), mas que foram desabilitadas para o RP1 (e.g. folha de rosto(?), ficha catalográfica, resumo/abstract, folha de aprovação)
 
## Interno

Convenções:

- coloque a seguinte `vim modeline` no final de cada `.tex`:

        % vim: tw=80 et ts=2 sw=2 sts=2 ft=tex spelllang=pt_br,en

- prefixe labels de imagens com `fig:`
- prefixe labels de equações com `eq:`
- prefixe labels de capítulos com `cap:`
