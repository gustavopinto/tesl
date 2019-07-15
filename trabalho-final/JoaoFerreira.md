# Relatório do Trabalho Final - NOME

* Nome completo: João de Deus Ferreira Filho
* Nível: Graduação
* Matrícula: 201504940020
* [Trabalho em Duplas](../duplas/Dupla_JOÃO_THIAGO.md)

## Reportar bug

* Mesmo quando usado um token pessoal, a CLI pede usuário e senha ([mathdroid/crop-github-images-cli#5](https://github.com/mathdroid/crop-github-images-cli/issues/5).
* O desenvolvedor não seleciona os arquivos específicos a serem publicados com o pacote gerando uma build com peso desnecessário ([pandrRe/Fastable#2](https://github.com/pandrRe/Fastable/issues/2)).

## Corrigir bug

* O gerador de site estático usava os repositórios do usuário no site mas não contava que quando o usuário não tivesse repositórios um erro era ocasionado ([saberland/create-portfolio#26](https://github.com/saberland/create-portfolio/pull/26)).
* O gerador de site estático não tinha suporte para links com `#fragment-identifiers` pois na build ele considerava apenas o link ao arquivo original ([saberland/saber#270](https://github.com/saberland/saber/pull/270)).
* O parser não conseguia identificar corretamente o início de um link em markdown ([saberland/saber#278](https://github.com/saberland/saber/pull/278)).

## Adicionar pequena funcionalidade

* Aponta qual o comentário com melhores reações (baseado em uma heurística simples) em uma issue do GitHub para facilitar encontrar possíveis respostas ou destaques importantes de se ler ([sindresorhus/refined-github#2108](https://github.com/sindresorhus/refined-github/pull/2108)).
* Incrementa a funcionalidade do ponto anterior adicionando uma _label_ no comentário em destaque ([sindresorhus/refined-github#2177](https://github.com/sindresorhus/refined-github/pull/2177)).
* Implementa a possibilidade da biblioteca NodeJs chamada `create-site` usar [templates do GitHub](https://help.github.com/en/articles/creating-issue-templates-for-your-repository) ([saberland/saber#271](https://github.com/saberland/saber/pull/271)).

## Adicionar grande funcionalidade

* Cria uma nova regra do eslint que adiciona a possibilidade de se passar argumentos a comentários _TODO_ e definir condições em que eles se tornam inválidos (data de expiração, biblioteca adicionada/removida, versão de certa tecnologia entre outros) ([sindresorhus/eslint-plugin-unicorn#302](https://github.com/sindresorhus/eslint-plugin-unicorn/pull/302)).
