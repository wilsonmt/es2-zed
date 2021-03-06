# Zed

## Introdução
Este é um trabalho para a disciplina de Engenharia de Software II, onde foi solicitado que fosse escolhido um projeto de código aberto presente no repositório GitHub com a finalidade de documentá-lo. O projeto selecionado selecionado foi o Zed, que é um editor de texto que pode alterar arquivos locais e remotos em qualquer servidor. Ele desenvolvido por meio de tecnologias web e apresenta significativa relevância devido ao grande número de estrelas  e de colaboradores que possui, além da sua utilidade para desenvolvedores e pessoas que queriam ingressar na área de desenvolvimento.

## Descrição do Sistema
Zed é um editor de texto que foi desenvolvido utilizando tecnologias web, funcionando como um app do Chrome. De acordo com os desenvolvedores, o editor foi projetado com a ideia de repensar algumas características que permeiam os atuais editores de texto. Segundo eles, algumas das principais características do editor Zed são justamente as funcionalidades que ele não possui, como tabs, árvore de arquivos sempre visível, menus, botões, sinos e apitos.
 
Essas funcionalidades, comumente utilizadas em outros editores de texto, foram removidas com o objetivo de tornar o editor mais simples e intuitivo. Com essa proposta minimalista a intenção é se concentrar no que mais importa, tornando o processo de codificar menos burocrático e mais produtivo.
O editor funciona como um app sobre a engine do navegador Google Chrome, mas também pode ser compilado localmente, funcionando no Mac, Linux, Windows e todos os sistemas que suportam o navegador Chrome.

## Funcionalidades da aplicação
Algumas funcionalidades incluídas com o objetivo de agregar valor foram:

* Múltiplos cursores: é uma funcionalidade que permite que o usuário edite várias partes do código simultâneamente, funciona bem em refactors mais simples, como em nomes de variáveis, por exemplo.
* Navegação no projeto com vários níveis de granularidade: funciona para alternar rapidamente entre arquivos e acessar grupos deles de acordo com seus símbolos.
* Auto atualização da visualização para várias linguagens: ao atualizar o arquivo, há a visualização em tempo real das mudanças feitas, duas das linguagens suportadas são Markdown e Coffeescript.
* Edição de arquivos locais ou remotos, como o software funciona como um Chrome App, os arquivos locais são acessados via APIs específicas do Chrome, os arquivos remotos são acessados através de um servidor remoto, há também a possibilidade de acessar arquivos hospedados no Dropbox.

## Informações da equipe de desenvolvimento
Desde o seu início, já se passaram ao todo pelo time de desenvolvimento do Zed 40 contribuidores. Destes, podemos visualizar uma relação de participação de acordo com o número de commits por usuário no gráfico abaixo:
 
![](https://lh4.googleusercontent.com/NPd-JkwxAq_d98kfDvPavA6lJ8dGxkLFfQF-_LbKCNN10lyFap9Y5zwOESXH3JzWXybMMSQ2ky4suYiFqzzGXxN_mB3td-Mj42dTgaKPV2AkauFnuvgDUJPPn8IFqTlGzAab6_Uc)

Embora o número de contribuidores seja considerável, podemos observar que a maioria destes teve uma participação muito breve no projeto, sendo que, os contribuintes #37 e #40, por exemplo, fizeram um commit alterando apenas uma linha de código. O membro que mais contribuiu na aplicação foi, como o esperado, o autor dos códigos principais, Zef Hemel com um total de 698 commits.

### Zef Hemel
Zef Hemel é PhD em ciência da Computação pela _Delft University of Technology_ (2007–2011). Suas pesquisas incluem design e implementação de várias linguagens de programação, especificamente Linguagens de Domínio específico (DSL), assim como ferramentas para as mesmas. Trabalhou em duas linguagens principais: WebDSL (para o desenvolvimento rápido de aplicações Web) e mobl (desenvolvimento rápido de aplicações Web para dispositivos móveis). O Zed foi um de seus principais projetos paralelos.
No gráfico abaixo, está representada a linha do tempo dos commits do programa desde o seu início em 2013. Podemos perceber que após o ano de 2015 a movimentação sobre o programa em geral foi bastante reduzido, sendo que, de 2016 até o momento atual não são indicadas nenhuma alteração nos registros do GitHub.

![](https://lh6.googleusercontent.com/EvNlypeY63fXMuOQy2daYhy3-MV4v_wtXlpfA_-FCd9FeoSe2GxcKF9HNkXOiVkscsgaGzqeltBgWz_xRrMbe5zusTxXP1oh9lwYbSFwEil-v1mJf3-SPbSK3ZcErc4H42zAiFwU)

Evidenciando uma possível diminuição no fluxo de alterações nos últimos dois anos, o gráfico abaixo representa o número de adições e deleções por semana desde o começo do aplicativo e ele nos confirma que depois de 04/15 não há mais alterações implementadas no Zed.

![](https://lh5.googleusercontent.com/vqmkbsA1Jq2yPTB69qknZZ1Re2PKqVOhyThDfV3gV0LY_3W-M1kQ-YInawxoXdNK-bqhnt1aVXi8UfkHh8s4l9deWV0cifMjMu9PAJiUIwxwm7867yGtZ8V_apXTv87LEhS8sovX)


## Descrição da evolução do sistema 

### Branches
Atualmente no GitHub, o Zed conta com quatro branches:

* master
* zedd
* mwjs
* rx

## Principais frameworks, ferramentas e linguagens usadas no desenvolvimento
Os desenvolvedores e colaboradores do Zed utilizam o GitHub como plataforma de hospedagem de código, para controle de versão e colaboração, além disso possuem uma web page com todas as informações necessárias, tanto para o uso do aplicativo como também para colaborar com o desenvolvimento do projeto.

Na implementação dessa ferramenta de edição são utilizadas diversas linguagens de programação, as linguagens de propósito geral usadas são: JavaScript (82.9%) e Python (porcentagem não significativa. Já as DSL (Domain Specific Language) usadas são  CSS (8,4%), e  HTML (8.1%) , além de JSON em menor escala. 

O editor de cógido usado foi o Ace (https://github.com/ajaxorg/ace) que é um editor de código autônomo escrito em JavaScript, e pode ser facilmente incorporado em qualquer página da Web ou aplicativo JavaScript. Algumas de suas funcionalidades são: sintaxe para mais de 120 idiomas, manipula documentos enormes (no último cheque, 4.000.000 linhas é o limite superior), pesquisar e substituir por expressões regulares e arraste e solte texto usando o mouse, além de apresentar verificador de sintaxe em tempo real (atualmente JavaScript / CoffeeScript / CSS / XQuery).

Também foram usadas outras ferramentas para o desenvolvimento do Zed, por exemplo o Architect que auxilia em aplicações Node.js, configurando os plugins do projeto. É uma estrutura simples criada pelos desenvolvedores cujo código é aberto. No entanto é poderosa para aplicações Node.js, pois usando esta ferramenta, você define uma configuração simples e mostra ao Architect quais plugins você deseja carregar. Cada plugin se registra com o Architect, então outros plugins podem utilizar as suas funções. Cada plugin é um módulo de nó completo com um arquivo package.json. e  podem ser mantidos em pacotes NPM para que possam ser descartados em outras aplicações do Architect, no entanto não há necessidade de realmente estar em NPM, pode ser uma pasta simples na árvore de código.

![](https://lh4.googleusercontent.com/2HAcRULPgn98n5SH04Hmyj4p-HMbB2taD66L1uX1_jCqYgGP0ZT2oKSxNEduLjs_yOIu3sqJ9LnNdBF0LdL46bohvv8sdx8wFRONkt4NOWCJmiJ8KdmOdAd9I9iq1mSL1bSVXwAz)

O jQuery também foi usado no desenvolvimento da aplicação, sabendo-se que o JQuery é uma biblioteca JavaScript, pequena e rica em recursos. Ele torna as coisas como documentos HTML, manipulação de eventos, animação e Ajax muito mais simples, por meio de uma uma API simples de usar, além disso ele funciona em diversos navegadores. Através de uma combinação de versatilidade e extensibilidade, o jQuery auxilia muitos desenvolvedores a escreverem códigos em JavaScript de uma forma mais eficiente.

Uma outra biblioteca do JavaScript usada é o  Underscore.js que fornece diversos ajudantes úteis de programação funcional sem estender os objetos internos. Isso possibilita tornar o código do projeto mais conciso, simples e correto. Essa biblioteca fornece mais de 100 funções que suportam funções funcionais comuns,  como: map, filter e invoke, bem como funções mais especializadas: ligação de função, javascript templating, criação de índices rápidos, teste de igualdade profunda, entre outros.

Podemos citar também o RequireJS (http://requirejs.org/) que executa arquivos e módulos do JavaScript, além disso ele é otimizado para o uso no navegador, no entanto esse aplicativo pode ser usado em outros ambientes JavaScript, como o Node. De acordo com o site dessa aplicação, usando um executor de script modular como RequireJS irá melhorar a velocidade e a qualidade do seu código, desse modo o desempenho do programa pode aumentar.

## Arquitetura
Podemos separar os aspectos arquiteturais aplicativo Zed em alguns tópicos, que possuem a seguinte hierarquia:

![](https://lh6.googleusercontent.com/vuQRXJ6xfCzCHLVkNhgCNM6YzFsbbF1qtjh0syYuduIhJt4zG3SIuS2b8ug5mZ_Bc5JqX1yGXNQiHKnRE-5_XRuWCFyb5MFY2-1PtPKD7Z7sObqAfix5MepNilf5YR38tHg66JdP)

### Chrome App
Chrome App é um tipo de aplicação que funciona através do Google Chrome. Essa aplicação aproveita a engine do Chrome e executa sobre os sistemas que possuem suporte ao navegador. Dessa forma, as possibilidades ao desenvolver dessa forma se expandem com relação a um simples site Web. Por questões comerciais alguns apps ficaram restritos somente a Chromebooks, o que não é o caso da aplicação que estamos documentando.

No caso do Zed o Chrome app é o aplicativo em si. Sua composição geral consiste em três tipos diferentes de janelas, que são:

* Lista de projetos: a lista de projetos é uma lista contendo os projetos que estão sendo manipulados pelo editor. É uma lista comum, contendo informações sobre o projeto e seus arquivos. Através dessa lista a navegação entre arquivos e projetos é possibilitada.
* Janela do editor: A janela do editor é onde se concentra o propósito geral do app, que é o código, essa janela possui funções especiais como o autocomplete inteligente (que é uma das features destacadas pelo desenvolvedores) e a atualização em tempo real para linguagens que trabalham com o aspecto visual, como Markdown e Coffeescript. 
* Janela para abrir arquivo através do Dropbox: Essa janela possui integração com as APIs do Dropbox, o que faz com que a natureza de sua implementação seja distinta das demais. 

![](https://lh4.googleusercontent.com/7QcP5DEeyXARuTDt_plQfxyy3DnJUQ6hH-Sh7vdHzSF7MdWQrPsG3BM-WIEVOaVPQ0GMhw_9U6AVuoaBaXjiyX7YoBEb1zzn5v_tq4TF4PhHN0uKv1zjOG_vyuHrEyMQ39yiJiJm)

### Comunicação cliente/servidor 
A comunicação cliente/servidor é feita nos arquivos com a extensão _.go_ contidos na raiz do projeto. Dependendo da situação o arquivo _zed.go_ atuará no modo servidor ou cliente.

O servidor atua como um proxy entre e o cliente e o Chrome App. Quando o Zed está em modo cliente, ele se comunica com o servidor Zed através de uma conexão websocket. O servidor disponibilizará os arquivos através do protocolo WebFS Desta forma, com um servidor Zed os arquivos podem ser editados remotamente.

### WebFS
O protocolo WebF (ou Web File System) é um protocolo usado pelo Zed para se comunicar com um servidor, podendo ser um servidor remoto ou local. Esse protocolo é extremamente simples e foi projetado para ser o mais direto possível, sem contar com muitos detalhes além de seu objetivo central.

### Inicialização do editor
A inicialização do editor se dá pelo seu arquivo principal. O arquivo principal do editor é o arquivo _editor.html_ que fica na pasta _app_. Sua função principal consiste em carregar algumas bibliotecas de dependência e o ponto de entrada principal, que é o arquivo _boot.js_, contido na pasta _app/js_.

### Eventbus 
Eventbus é uma espécie de central de envio de eventos, onde um módulo pode declarar um evento emiti-los ou ouvi-los em eventos. É usado em tarefas como alterar configurações do editor, criar um novo arquivo, alternar entre seções, entre outros.

### Comandos 
Os comandos são a base da interação com o usuário, quase todas as ações do mesmo se dão através de comandos. Existem comandos para abrir arquivos, fechar arquivos, alternar entre eles, salvar, fechar o editor, e muitas outras ações, sendo os mesmos primordiais para o funcionamento completo do editor. 

A implementação dos comandos do Zed está contida no arquivo _command.js_, que por sua vez se encontra na pasta _app/js_. Existem também os atalhos, através deles os comandos são executados por padrão através da combinação de teclas _Ctrl/Command + tecla chave_. Na imagem abaixo podemos ver alguns dos comandos presentes no editor:

![](https://lh3.googleusercontent.com/5dxmbLdkC2qAT8D2xlR5BiRR48B4aKqKfqkrQrt53KU7anrNl2Jh3D7AZs1hfiyuoOR3nD8NZJw_tSRv1eMmF1BEKpMR-Z1L5UzE5KwTGRjaw-d_nqPnghlyF0hz9nZiy4uuXpDT)

## Requisitos não-funcionais
Os requisitos não funcionais representam a parte técnica do sistema, como  portabilidade, usabilidade, desempenho, entre outros. Desse modo, iremos apresentar e discutir alguns desses requisitos, já que são importantes para a documentação da arquitetura do sistema. Em relação à portabilidade, o Zed funciona como um aplicativo sob a engine do Chrome, como se fosse uma extensão do navegador,  mas também ele pode ser compilado localmente off-line, dessa maneira, o usuário pode utilizá-lo nos sistemas operacionais Linux e Windows e em máquinas Mac. Também este editor permite leitura e gravação em serviços remotos como Github ou Dropbox, por exemplo. Podemos afirmar que esse aplicativo apresenta muito boa portabilidade, pois pode ser usado na maioria dos dispositivos comerciais.  

Com relação à usabilidade, podemos considerar que o usuário desse editor é pelo menos intermediário, pois presume-se que possui ao menos um conhecimento básico em programação. A partir disso, podemos considerar que o aplicativo não possui problemas graves de usabilidade, os termos e os símbolos utilizados são familiares aos usuários, além disso a interface parece ser bastante amigável aos programadores. Logo após a instalação por meio do Chrome Web Store - Extensões, irá aparecer uma tela para que o usuário já possa escolher entre um formato de editor mais simples, sem menus aparentes, ou um formato similar aos editores comuns, como o Sublime, como pode ser observado na imagem logo abaixo:

![](https://lh5.googleusercontent.com/Iz4IK5h_FUOh1mlh33N0BuOklHvUytR_cuLWZsMh4TGupymV4sMzDumnOLnQPOAB8Eq3EVKdikWwlTi4kO8YP3tZqTj4dbMCAMcDinvQ56fD-9Tf4LWakQujZjHW8P_BQB122gj0)

Após escolher o formato desejado, basta clicar em “Start using Zed” para começar a usar o editor. Um problema de usabilidade encontrado é que o usuário precisa ter ao menos um conhecimento básico na língua inglesa para poder usar e entender todas as funcionalidades desse editor de texto. A escolha de esquema de cores do editor foi adequada, pois há alto contraste, e além disso as cores são perceptíveis aos  daltônicos.

Em relação ao desempenho, pode-se dizer que este editor pode ser comparado a aqueles mais utilizados pelo programadores, como o Sublime e o o Atom. Um outro requisito não-funcional que podemos citar é a interoperabilidade, o Zed funciona tanto com repositórios, como o GitHub e o DropBox, como arquivos locais e remotos. Já em relação a segurança que é um outro requisito não-funcional, podemos dizer que é um aplicativo seguro, mas que depende do usuário manter senhas confiáveis do Chrome, e dos repositórios que possui, dessa forma os arquivos mantidos no Zed só poderão ser acessados por terceiros se souberem a senha ou se invadirem  o computador e os arquivos estiverem sem a devida proteção.

## Mecanismos arquiteturais
Neste ponto, iremos listar alguns dos mecanismos arquiteturais encontrados no aplicativo.

 
MECANISMO DE ANÁLISE       | MECANISMO DE DESIGN                               | MECANISMO DE IMPLEMENTAÇÃO
---------------------------|---------------------------------------------------|----------------------------
Front-End                  |Interface de comunicação com o usuário do portal.  |CSS, HTML, JavaScript
Build                      |Programação da IDE para validação do código fonte. |ACE e Architect
Deploy                     |Configuração da IDE de deploy.                     |ACE e Architect
Recursos avançados de Web  |Implementação de recursos para usabilidade.        |CSS e JavaScript


## Problemas de implementação
Ao longo do desenvolvimento do aplicativo, vários bugs e outros tipos de problemas foram encontrados pelos colaboradores principais, e também pelos muitos usuários e outros colaboradores do projeto que reportam falhas. Ao fazer uma leitura rápidas desses problemas, percebe-se que não são usuários iniciantes que reportam essas falhas, devido ao nível de conhecimento necessário para poder fazer tais relatos.

Esses problemas estão todos em ordem cronológica, no entanto é possível aplicar filtros para possibilitar a visualização de problemas específicos. Os filtros apresentados pelo GitHub são:

* Autor:  são mostrados quatro autores, provavelmente são os mais frequentes;
* Etiquetas: são diversas etiquetas, ACE Bug, api, bug, Chrome bug, duplicado, aprimoramento, feedback requerido, inválido, atalhos de teclado, baixo nível, prioridade baixa, problemas menores, propostas e perguntas.
* Versões: são apresentadas três opções, problemas sem versão e as duas versões do aplicativo.
* Administradores: são apresentadas novamente quatro opções.
* Ordenado por: neste filtro são mostradas opções de ordenação, por exemplo do mais recente ao mais antigo.

Nesta parte do trabalho, vamos comentar alguns dos bugs e problemas encontrados resolvidos e outros ainda abertos:

* Impossible to open last-opened folder in Zedd #513 (Impossível abrir a última pasta aberta no Zed): um usuário reportou que ao tentar abrir uma pasta pelo Zed, a última que está selecionada, por padrão, ele não conseguiu selecionar esta pasta para abri-la, e ao tentar desmarcar esta pasta, também não obteve sucesso. O desenvolvedor principal corrigiu o bug logo em seguida.
* "Info" annotation looks bad in dark window theme #504 (A anotação "Info" parece estar ruim no tema da janela escura #504): um ícone era muito estava muito pequeno e não apresentava contraste com o tema escuro do aplicativo. Um ponto interessante é que o foi um dos desenvolvedores principais que reportou e ele mesmo corrigiu o problema esse problema de usabilidade. O desenvolvedor principal corrigiu o bug logo em seguida.
* Zed's keybindings don't work in ACE's "normal" vim mode#487 (As combinações de teclas do Zed não funcionam no modo vim "normal"  do ACE #487) : um usuário relatou que  as combinações de teclas, como  Ctrl+F e Ctrl+E, não estavam funcionando no modo vim normal, o usuário precisaria entrar no modo de inserção para poder usar esses atalhos. Essa é uma funcionalidade importante em editores de texto para programadores, já que usar atalhos é uma prática usual para quem está acostumado a escrever códigos. O desenvolvedor principal atendeu a requisição e corrigiu o bug logo em seguida.
* Feature Request: Templates #592: nessa requisição o usuário está sugerindo que o Zed possua um template similar ao Sublime ou a outros editores de texto.
* Disconnects from Dropbox when Creating a new file #589 (Desconecta do Dropbox ao criar um novo arquivo # 589): o usuário está reportando que não está conseguindo criar um arquivo em um diretório do Dropbox sem falhas no cliente.
* Zedapp randomly zooms in on mac #586 (O Zed está aleatoriamente acionando o zoom em computadores Mac): o usuário reportou um comportamento estranho do aplicativo ao ser usado em computadores Mac, ele relata que ao usar o modo tela cheia um zoom é aplicado inesperadamente às vezes, impossibilitando o uso do menu. 
  
## Casos de uso
Com a finalidade de exemplificar situações em que o Zed pode ser utilizado, vamos descrever dois casos de uso:

* “Clarisse, de 22 anos de idade, estudante de Sistemas de Informação necessita escrever um projeto para uma atividade de extensão na qual está participando. Ele decidiu escrever uma extensão do Chrome que possui como funcionalidade principal  identificar linguagens de programação em arquivos diversos. Dessa forma, ela decidiu ir na loja virtual do Chrome para procurar por um bom editor de texto gratuito bem avaliado pelos usuários, então ela encontrou o Zed e resolveu testá-lo.”
* “Joesly, de 36 anos, desenvolvedor web pleno na empresa GBS Comissões, recebeu uma requisição da gerência para desenvolver um sistema de tempo real para controlar as finanças da empresa, com a finalidade de automatizar a contabilidade da empresa e poupar despesas com serviços terceirizados. Ele já estava acostumado a utilizar o editor de texto Sublime, no entanto ele decidiu  testar um outro editor e foi procurar no Google outras alternativas. Dessa forma, ele encontrou o Zed e se interessou  pela descrição dele, como ele possuía um prazo de entrega relativamente longo, ele decidiu testá-lo.”
