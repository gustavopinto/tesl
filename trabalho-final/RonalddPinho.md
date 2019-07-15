# Relatório do Trabalho Final - RONALDD PINHO

* Nome completo: RONALDD PATRIK SILVA PINHO
* Nível: Graduação
* Matrícula: 201704940035
* [Trabalho em Duplas](duplas/Dupla_RONALD_WAGNER.md)

## Correção de Bug (3 pts)

* Includes absolutos nos códigos fontes do módulo EO causava inconsistência na inclusão desse módulo no código fonte do usuário, os includes deveriam ser relativos como apontava uma issue do proprio mantenedor do projeto. Mudei para includes relativos dentro dos códigos fontes e acabaram todos os erros de compilação e inclusão referentes às inconsistências de includes. PR ([ParadisEO#43](https://github.com/nojhan/paradiseo/pull/43)).

## Traduções 2x (2 pts)

* Traduzi alguns arquivos de documetação do projeto Brython para português brasileiro. PR
([Brython#1151](https://github.com/brython-dev/brython/pull/1151));

* Traduzi (iniciei um processo de tradução) no projeto de um framework de testes em C++ conhecido como [Catch2](https://gihub.com/catchorg/Catch2), pretendo traduzir todos os arquivos de documentação e tutoriais para o português brasileiro. PR [Catch2#1675](https://github.com/catchorg/Catch2/pull/1679).

## Bug Report 2x (2 pts)

* ParadisEO aprensenta erros nas execuções de testes do módulo MO, reportado em [ParadisEO#44](https://github.com/nojhan/paradiseo/issues/44);

* A biblioteca de Funções estatísticas da linguagem Julia apresenta erros em um de seus testes. [StatsFuns#74](https://github.com/JuliaStats/StatsFuns.jl/issues/73).

## Melhoria na documentação (1 pt)

* Arquivos Markdown são mais fáceis para trabalhar, uma [issue](https://github.com/cookiecutter/cookiecutter/issues/1179) no projeto [Cookiecutter](https://github.com/cookiecutter/cookiecutter) pede para converter os arquivos de doc .rst para .md. PR [Cookiecutter#1188](https://github.com/cookiecutter/cookiecutter/pull/1188).
