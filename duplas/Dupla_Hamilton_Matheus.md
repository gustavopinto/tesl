
# Dupla

- Hamilton Cavalcante (hamiltoncavalcante@gmail.com)
- Matheus Seabra (matheusvieiracoelho@gmail.com)

### Links para atividades:

## Atividade 01:
- 

## Atividade 02: 
- 

## Atividade 03

1. **Experimente os comandos do `git` em algum repositório de código. Utilize os commandos `commit`, `push`, `pull`, `checkout`, `log`, `shortlog`, etc. Descreva o que cada um desses comandos faz**.

- commit: uma operação que descreve certa mudança/incremento/exclusão de código
- push: Envia mudanças locais para o reposiório origem
- pull: puxa mudanças localmente do repsotório de origem
- checkout: alterna entre branches
- log: exibe uma série de informações sobre a mudança
- shortlog: exibe um log mais curto sobre as mudanças

2. **Baixe o site da disciplina na sua máquina local, e rode um comando para imprimir uma saída de terminal similar a esta:**

	R = git shortlog -n -e 

## Atividade 04

### 1. Selecione e identifique em um determinado projeto de software livre se a página inicial ou alguma página logo em seguida tem (ou não) links para instalação, documentação, documentação traduzida, e como contribuir. Coloque o projeto avaliado e os links encontrados (ou não).

**Projeto: Cypress.io**
Função do projeto: JavaScript End to End Testing
Link do repositório: https://github.com/cypress-io/cypress
Link para documentação: https://docs.cypress.io
Link de como contribuir: https://github.com/cypress-io/cypress/blob/develop/CONTRIBUTING.md
Template para abrir Pull Request: https://github.com/cypress-io/cypress/blob/develop/PULL_REQUEST_TEMPLATE.md
Código de conduta: https://github.com/cypress-io/cypress/blob/develop/CODE_OF_CONDUCT.md
Link para o FAQ: https://docs.cypress.io/faq/questions/using-cypress-faq.html
Link para Traduções: não possui link

### 2. Revise uma página de um projeto de software livre e sumarize os problemas encontrados (o que falta para ela ser mais informativa)

**Projeto: Mongoose**
Link para o repositório: https://github.com/Automattic/mongoose
Link para documentação: 
Problemas encontrados:
- Falta página de traduções
Sugestão de como melhorar:
- Adicionar página de tradução
- Adicionar página de código de conduta
- Adicionar template de Pull request
- Adicionar template para issues 


### 3. Teste a documentação (por exemplo, siga as instruções de instalação) e sumarize os problemas encontrados.

Documentação: https://docs.cypress.io

Passos para instalação: 

passo 1: Instala a blibioteca globalmente e como dependência de desenvolvimento
```npm install cypress -g --save-dev``` 

passo 2: Abre o terminal interativo para executar os testes 
```npm run cypress open```

Problema encontrado: o Cypress ainda não possui uma maneira de simular cliques os outros eventos do navegador de forma condicional. Isso acontece pois o DOM nas aplicações usando JavaScript de hoje se torna incrivelmente instável. Portanto, o Cypress tem dificuldade em saber quais elementos HTML estão em telas e os que não estão, fazendo com que alguns testes podem ser considerados "frágeis", ou seja, não consistentes, e podem falhar por razões aleatórias.

## Atividade 05

### 1. Justifique o que acontece se um projeto de software não tiver nenhuma licença definida.

R = Se um projeto não possui licença, então não é considerado open source. Se não tiver uma licença que conceda ao usuário do software direitos específicos além dos direitos concedidos a ele/ela pela lei de direitos autorais (que são praticamente nenhum), então ela não é de código aberto. Em particular, não seria possível ter permissão para copiá-lo, modificá-lo, distribuí-lo, nem baixá-lo, etc. Dependendo da jurisdição, pode-se nem ter permissão para executá-lo, pois a execução envolve a cópia do disco para a RAM; a maioria das jurisdições, felizmente, se afastou dessa interpretação, mas ainda pode haver algumas que não foram.

Nota do GitHub sobre o assunto: https://help.github.com/en/articles/licensing-a-repository#what-happens-if-i-dont-choose-a-license

>You're under no obligation to choose a license. It's your right not to include one with your code or project, but please be aware of the implications. Generally speaking, the absence of a license means that the default copyright laws apply. This means that you retain all rights to your source code and that nobody else may reproduce, distribute, or create derivative works from your work. This might not be what you intend.

>Even if this is what you intend, if you publish your source code in a public repository on GitHub, you have accepted the Terms of Service which do allow other GitHub users some rights. Specifically, you allow others to view and fork your repository.

>If you want to share your work with others, we strongly encourage you to include an open source license.

### 2. Procure um projeto sem licença de software e adicione uma

Projeto: https://github.com/matheuseabra/js-dev-tools
Licença: GNU General Public License v3.0
Link da licança no repositório: https://github.com/matheuseabra/js-dev-tools/blob/master/License.md

3. Procure por projetos de software que utilize uma licença que não deveria ser empregada em projetos de software.

Projeto: https://www.freertos.org/

Como exemplo, o sistema operacional em tempo real FreeRTOS é licenciado sob a Licença Open Source do FreeRTOS que é baseada em uma GNU GPL modificada, a modificação assumindo a forma de uma exceção. A GNU GPL é aprovada pela Open Source Initiative, mas não pela FreeRTOS Open Source License.

## Atividade 06

### 1. Encontre Roadmaps em pelo menos 3 projetos de software livre. Descreva os planos de curto e longo prazo desse projeto

**Projetos**: 

**TypeScript Roadmap** (https://github.com/Microsoft/TypeScript/wiki/Roadmap)
 
 **Curto prazo**:
 - Types on every desk, in every home, for every JS developer
 - Productivity through strong tooling  
 - Approachability and UX        
 -  Community engagement   
  - Infrastructure and engineering systems

  **Longo prazo:** 
   - Variadic types
   - Investigate nominal typing support
   - Flattening declarations
   - Implement ES Decorator proposal
    - Implement ES Private Fields
    - Investigate Ambient, Deprecated, and Conditional decorators
    - Investigate partial type argument inference
    - Quick fix to Scaffold local @types packages
   - Investigate error messages in haiku or iambic pentameter
    - Decorators for function expressions/arrow functions

 **React Roadmap** (https://reactjs.org/blog/2018/11/27/react-16-roadmap.html)
  **Curto prazo**:  -   React 16.6 with  [Suspense for Code Splitting](https://reactjs.org/blog/2018/11/27/react-16-roadmap.html#react-166-shipped-the-one-with-suspense-for-code-splitting)  (_already shipped_)
-   A minor 16.x release with  [React Hooks](https://reactjs.org/blog/2018/11/27/react-16-roadmap.html#react-16x-q1-2019-the-one-with-hooks)  (~Q1 2019)
-   A minor 16.x release with  [Concurrent Mode](https://reactjs.org/blog/2018/11/27/react-16-roadmap.html#react-16x-q2-2019-the-one-with-concurrent-mode)  (~Q2 2019)
-   A minor 16.x release with  [Suspense for Data Fetching](https://reactjs.org/blog/2018/11/27/react-16-roadmap.html#react-16x-mid-2019-the-one-with-suspense-for-data-fetching)  (~mid 2019)
  
  **Longo prazo:** 

**Babel** (https://babeljs.io/docs/en/7.1.0/roadmap)
 **Curto prazo**: 
 -   There is also  [https://github.com/mdn/browser-compat-data](https://github.com/mdn/browser-compat-data)
-   Also use data from test262?
-   Run tests against real browsers
-   have a data-only format
-   Need continued maintainence
- 
  **Longo prazo:** 

### 2.  Selecione 5 projetos de software livre famosos (pelo menos 1000 estrelas) e coloque os links para seus respectivos site, repositório de código fonte, bug tracking e ferramentas de comunicação

Projeto: **Apollo GraphQL - A community building flexible open source tools for GraphQL.**
Site: [https://www.apollographql.com/](https://www.apollographql.com/)
Repositório: [https://github.com/apollographql](https://github.com/apollographql)
Bug tracking: [https://github.com/apollographql/apollo-server/issues](https://github.com/apollographql/apollo-server/issues)
Chat: [https://spectrum.chat/apollo?tab=posts](https://spectrum.chat/apollo?tab=posts)

Projeto: **Express - Fast, unopinionated, minimalist web framework for Node.js**
Site: [https://expressjs.com](https://expressjs.com/)
Repositório: [https://github.com/expressjs/express](https://github.com/expressjs/express)
Bug tracking: [https://github.com/expressjs/express/issues](https://github.com/expressjs/express/issues)
Chat: [https://gitter.im/expressjs/express](https://gitter.im/expressjs/express)

Projeto: IPFS - Peer-to-peer Hypermedia Protocol 
Site: [https://ipfs.io](https://ipfs.io/)
Repositório: [https://github.com/ipfs/ipfs](https://github.com/ipfs/ipfs)
Bug tracking: [https://github.com/ipfs/ipfs/issues](https://github.com/ipfs/ipfs/issues)
Chat: [https://discuss.ipfs.io/](https://discuss.ipfs.io/)


### 3.  Encontre e discuta formas de priorizar requisitos em projetos de software livre

Estratégias para gerenciar bugs em projetos de software livre:

- Faça seus bugs bem visíveis: 
- Priorize os bugs com labels
- Verificar se referem-se a um bug de software real,
- Verficar que bug reports não estejam duplicados
- O bug report deve conter informações suficientes para serem resolvidos imediatamente

## Atividade 09

### 1. Explique o são Linters e qual a sua importância ?

R = Linters são ferramentas para padronizar código de liguagens de programação em um formato/estilo. Os linters são importantes durante o processo de desenvolvimento de software pois essas ferramantas permitem que haja uma homogenização no formato entre todos os membros da equipe que estão participando daquele projeto. Além disso, outro resultado que linters trazem é uma redução de inconsistências no código do projeto.

### 3. Indique um guia de boas práticas de codificação em frameworks de linguagem de programação.

Linguagem: Python
Framework: Django

Boas práticas:

- Nomenclaturas:
  As boas-práticas de nomenclaturas dos models em Django seguem também as boas práticas da PEP8, que são, basicamente:

  Nomes de classes são capitalizadas;
  Nome dos métodos e atributos são em snake_case;
  Além disso, os nomes das classes devem ser sempre no singular. Isso se dá pois uma classe model representa um objeto daquele tipo de dado, e não uma coleção.

- Ordenação de atributos e métodos
  
  De acordo com a documentação oficial de boas práticas do Django, a ordem indicada para os métodos e atributos de uma classe são:

  - Constantes
  - Campos da tabela
  - Custom Managers
  - classe Meta
  - sobrescrição do __str__()
  - sobrescrição do __save__()
  - definição do get_absolute_url()
  - Properties customizadas
  - Métodos customizados

- Atenção para a diferença entre 'blank' e 'null': 

  É importante saber a diferença entre os atributos blank e null.

  null: é o atributo que corresponde a capacidade do campo aceitar valores nulos no banco de dados. Por padrão, todo campo criado no django não aceita valores nulos.
  blank: é o atributo responsável por lidar com a entrada deste dado, seja via django-admin ou forms. Você pode ter um campo que aceita valores nulos no banco de dados mas que não aceita uma entrada vazia no seu formulário.

- Use os 'Managers'

Semelhante aos modelos, é recomendável abstrair a lógica comum em métodos em um 'gerenciador'. Mais especifícamente, é provavelmente desejável um método que possa ser usado em cadeia e que possa ser usado em qualquer hora.

## Atividade 09

### 1. Explique o são métodos ágeis e qual a sua importância no processo de desenvolvimento de softwares ?

Os métodos ágeis são um modelo alternativo para gestão tradicional de projetos. Esse método fo desenvolvido em resposta ao modelo de processo em cascata, muito utilizado nos anos 90, porém que trouxe muitos prejuízos, não agregando valor para o cliente. Portanto, em 2001 foi criado o manifesto ágil, que explana todos os princípios e valores da metodologia ágil

As metodologias ágeis são um modelo alternativo para gestão tradicional de projetos, que estejam alinhadas com os valores e princípios descritos no Manifesto Ágil para Desenvolvimento de Software, assinado em 2001 em Utah. Participaram desse evento 17 desenvolvedores, que apesar de estarem testando abordagens e métodos diferentes, compartilhavam dos mesmos fundamentos. As metodologias ágeis em geral defendem o planejamento adaptativo, times auto-organizados e multidisciplinares, melhoria contínua e o desenvolvimento evolucionário. Se olharmos a forma como o desenvolvimento de software se dá em diversas empresas, veremos o oposto disso.

### 2. Procure um projeto e indique um commit que indique trabalho feito em par, ou seja, um commit que tenha multiplos autores 

Projeto: Hiptest publisher
Commit: https://github.com/hiptest/hiptest-publisher/commit/15b9b2cdf63b54bc0a4fcc36a60c7da47be0e7a6

### 3.Procure um projeto e indique um commit que contenha indícios da metodologia TDD (Test Driven Development), ou seja, o desenvolvedor enviou o código fonte com o teste no mesmo commit.

Projeto: Sails.js
Commit: https://github.com/balderdashy/sails/commit/661dfac93fbb08c9ae685066ae5b3da5eaa583f3#diff-098f6bcd4621d373cade4e832627b4f6

## Atividade 10

### 1. Por que utilizar testes unitários?

Teste unitários é um nível de testes em software onde partes e componentes individuais são testadas. 
O objetivo desse tipo de teste é validar cada que cada unidade de software funcione como foi projetado. 

### 2. Quais vantagens de utilizar integração contínua?

A intengração contínua ajuda times de desenvolvimento de software a serem mais produtivos de acordo com a metodologias ágeis, permitindo que times consigam responder a mudanças de requisitos de negócio rápidamente, e ao mesmo tempo garantindo que o hardware e software estejam sincronizados constantemente entre si. A CI permite que membros de uma mesma equipe trabalhem focados em seus domínios, focando em tarefas que se sobresaem melhor para entregar, dando a confiança para o time que as contribuições estão integradas e que os componentes funcionam como esperado. E se algo no sistema não está integrado, pode ser rapidamente descoberto.

### 3. Adicionar um serviço de integração contínua (Travis) em um projeto pessoal.

# Atividade 11

### 1. Explique detalhadamente qual é a diferença entre as métricas "truck factor" e "heroes"

A métrica truck factor refere-se a concentração de conhecimento, acoplamento e dependência de um projeto de software livre em um contribuidor específico. Essecialmente o truck factor mostra se há algum gargalo na forma de contribuições centralizadas na mesma pessoa, o que pode ocasionar silos de conhecimento para o projeto. Já os heroes, são contribuidores que possuem o maior nível de contribuições em um projeto de software livre, geralmente tais heróis possuem conhecem a arquitetura do software de forma ampla e possui contribuições em diversos aspectos do projeto.

### 2. Cite pelo menos tês outras métricas de saúde de projetos de software livre

- First time, casual, and repeat contributors 
- Number of open issues and pull requests opened
- Average time a issue remains open
- Average time to merge a pull request

### 3. Explique porque os meios para medir qualidade de um projeto de software "tradicional" tem pouca aderência em projetos de software livre?

- As métricas de software proprietário tradicional não podem ser usadas como critérios acurados para avalidar software livre, pois esse forma de criar software possui aspectos nas quais software proprietário não possui, como comunidade e etc. 
