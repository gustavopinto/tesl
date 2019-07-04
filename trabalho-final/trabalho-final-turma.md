# Trabalho Final - Turma

Esse arquivo compila **todas as colaborações*- realizadas pela turma durante a realização do trabalho final.
O propósito deste arquivo é permitir uma visão global de tudo o que foi desenvolvido, de maneira simples e rápida.

As colaborações estão divididas por tipos, conforme estabelecido na [especificação do trabalho final](../trabalho-final.md), e devem seguir o seguinte padrão:

`- frase descrevendo o que foi feito ([link para a colaboração]() - [@usuario]())`

Por exemplo:

- Permite que o OpenDSSDirect busque o caminho para o GCC independente da distribuição ([OpenDSSDirect#24](https://github.com/Muxelmann/OpenDSSDirect.make/pull/24) - [@filipesaraiva](https://github.com/filipesaraiva))

Segue abaixo todas as colaborações realizadas pela turma durante a disciplina.

## Reportar bug

- Mesmo quando usado um token pessoal, a CLI pede usuário e senha ([mathdroid/crop-github-images-cli#5](https://github.com/mathdroid/crop-github-images-cli/issues/5) - [@lubien](https://github.com/lubien)).
- O desenvolvedor não seleciona os arquivos específicos a serem publicados com o pacote gerando uma build com peso desnecessário ([pandrRe/Fastable#2](https://github.com/pandrRe/Fastable/issues/2) - [@lubien](https://github.com/lubien)).

## Melhorar documentação

- Melhoramento de documentação do repositório,que ao investigar a documentação não ficava claro como instalar e rodar o ambiente local de desenvolvimento, após conversar com os mantenedores e abrir um issue, eles alteraram a wiki com instruções que eu criei ([issue #219](https://github.com/ryceg/Eigengrau-s-Essential-Establishment-Generator/issues/219#issuecomment-506033821), [Wiki deles após sugestão](https://github.com/ryceg/Eigengrau-s-Essential-Establishment-Generator/wiki/Compiling-the-Generator) - [@urielfcampos](https://github.com/urielfcampos))

## Realizar tradução

## Corrigir bug

- O gerador de site estático usava os repositórios do usuário no site mas não contava que quando o usuário não tivesse repositórios um erro era ocasionado ([saberland/create-portfolio#26](https://github.com/saberland/create-portfolio/pull/26) - [@lubien](https://github.com/lubien)).
- O gerador de site estático não tinha suporte para links com `#fragment-identifiers` pois na build ele considerava apenas o link ao arquivo original ([saberland/saber#270](https://github.com/saberland/saber/pull/270) - [@lubien](https://github.com/lubien)).
- O parser não conseguia identificar corretamente o início de um link em markdown ([saberland/saber#278](https://github.com/saberland/saber/pull/278) - [@lubien](https://github.com/lubien)).

## Adicionar pequena funcionalidade

- Pacote de um componente vue.js para animação de escrita, foi sugerido implementar a possibilidade de simular um cursor "falso", eu implementei como pedido. O cursor foi adicionado com a possibilidade de configurar a velocidade em que ele pisca, cor, formato e além de também adicionar uma classe css para infinitas configurações ([PR #6](https://github.com/trickstival/vue-typing/pull/6) - [@urielfcampos](https://github.com/urielfcampos))
- Aponta qual o comentário com melhores reações (baseado em uma heurística simples) em uma issue do GitHub para facilitar encontrar possíveis respostas ou destaques importantes de se ler ([sindresorhus/refined-github#2108](https://github.com/sindresorhus/refined-github/pull/2108) - [@lubien](https://github.com/lubien)).
- Incrementa a funcionalidade do ponto anterior adicionando uma _label_ no comentário em destaque ([sindresorhus/refined-github#2177](https://github.com/sindresorhus/refined-github/pull/2177) - [@lubien](https://github.com/lubien)).
- Implementa a possibilidade da biblioteca NodeJs chamada `create-site` usar [templates do GitHub](https://help.github.com/en/articles/creating-issue-templates-for-your-repository) ([saberland/saber#271](https://github.com/saberland/saber/pull/271) - [@lubien](https://github.com/lubien)).

## Adicionar grande funcionalidade

- Um projeto de auxílio para Dungeon masters de rpg de mesa, ele gera cidades e regiões inteiras, uma [issue](https://github.com/ryceg/Eigengrau-s-Essential-Establishment-Generator/issues/205), pedia para implementar uma nova funcionalidade que alterava a maneira que cidades eram geradas, incluindo um material de construcao "principal" para aquela cidade, que influencia o material das construções daquela cidade que acabavam ficando complementamente incoerentes por serem escolhidos aleatoriamente sem nenhuma influência da cidade em que se encontravam. Esta geração agora é influenciada pelo tamanho da cidade, riqueza e localização da mesma, depois de gerado, gera-se o material individual de cada construção da cidade, que é influenciada pelo material "principal" da cidade e pela riqueza do dono da construção.([PR #220](https://github.com/ryceg/Eigengrau-s-Essential-Establishment-Generator/pull/220) - [@urielfcampos](https://github.com/urielfcampos))
- Cria uma nova regra do eslint que adiciona a possibilidade de se passar argumentos a comentários _TODO_ e definir condições em que eles se tornam inválidos (data de expiração, biblioteca adicionada/removida, versão de certa tecnologia entre outros) ([sindresorhus/eslint-plugin-unicorn#302](https://github.com/sindresorhus/eslint-plugin-unicorn/pull/302) - [@lubien](https://github.com/lubien)).

## Desenvolver estudo original com artigo sobre software livre
