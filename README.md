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

Conferir se as linhas 156-218 estão comentadas

linha 84 de CMakeLists.txt precisa ter '_consideracoes.tex' em vez de 'cons_finais.tex'

Após as dependências estarem construídas, digitar os comandos:
`cd "pasta do projeto"`
`mkdir build`
`cd build`
`cmake .. && make pdf`

## Interno

Convenções:

- coloque a seguinte `vim modeline` no final de cada `.tex`:

        % vim: tw=80 et ts=2 sw=2 sts=2 ft=tex spelllang=pt_br,en

- prefixe labels de imagens com `fig:`
- prefixe labels de equações com `eq:`
- prefixe labels de capítulos com `cap:`
