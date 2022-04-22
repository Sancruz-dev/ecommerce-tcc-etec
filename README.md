<div align="center">

# Projeto Rivier - Loja Virtual de Joias

> Trabalho de Conclusão de Curso (TCC) proposto pela ETEC Jardim Ângela, criado a partir dos fundamentos e aprendizagens concedidas no curso de desenvolvimento de sistemas.

<image height="250" src="https://user-images.githubusercontent.com/83969467/163599582-9bbe5a67-a8e3-4645-8aca-2b00b3a8d433.png" alt="Ilustração introdutória da exposição do projeto" title="Ilustração introdutória"/>


</div>



### :warning: Avisos Importantes

Devido à motivos pessoais, Pamela (dona da Rivier Alianças), não pôde dar continuidade ao seu trabalho após o projeto ser entregue à ela, resultando na **DESATIVAÇÃO** da loja virtual de joias, até o momento.

Portanto, ainda é possível realizar cadastro/login, fazer comentários, avaliar/favoritar produtos, e algumas outras opções, posto que, não há como efeturar compras pelo website.

***

### Sumário

1. [Apresentação](#1-Apresentação)
   1. [Rivier-Aliancas](#i-Rivier-Alianças)
   2. [O Projeto](#II-O-Projeto)
2. [Desenvolvimento](#2-Desenvolvimento)
   1. [Prototipação](#i-Prototipação)
   2. [Sistema](#ii-Sistema)
   3. [Linguagens](#iii-Linguagens)
   4. [Hospedagem e CI/CD](#IV-Servidores-e-CI/CD)
   5. [Perfomance e API's](#V-Perfomance-e-APIs)
3. [Documentação](#3-Documentação)
4. [Referências](#4-Referências)

<br/>

## <div align="center"> 1. Apresentação</div>

Olá, sou Sanmir Cruz, líder da equipe responsável por criar esse sistema e-commerce, no qual, será apresentado no decorrer dos tópicos. Primordialmente, cabe destacar, que esse repositório exibirá as principais funções exercidas por mim (a partir do tópico de [Desenvolvimento](#2-Desenvolvimento)), dentro desse trabalho acadêmico, juntamente com as demais funcionalidades que o projeto emite.


### I. Rivier Alianças

<image height="332" src="https://user-images.githubusercontent.com/83969467/163585198-6e0d8067-0f97-498e-b68d-8c8986b03b98.png" alt="Introdução da empresa cliente" title="Introdução da empresa cliente" /> 

> _Introdução da empresa cliente_


Para conseguir vender seus produtos, Pamela dependia do uso das redes sociais apenas (como o Instagram, e Facebook), redirecionando seus clientes para o WhatsApp ou chats privados como Menssenger, para conseguir efetuar a venda. <br/> Suas opções de pagamento são: pix, mercado pago, boleto e cartões de crédito/débito.

<br/>

### II. O Projeto

###### <image src="https://user-images.githubusercontent.com/83969467/164773512-4ab2f251-07de-49c7-91ec-9ed15f98db09.png" alt="Abordagem das funcionalidades" title="Abordagem das funcionalidades" /> 

> _Abordagem às funcionalidades_


Para melhor compreensão, o sistema pode ser dividido em **duas grandes partes**:

- **Catálogo**: onde o público tem acesso, podendo fazer tudo o que a loja oferece (compras de produtos, cadastramento de conta pessoal, comunicações com o vendedor, comentários e avaliações sobre produto, e etc).

- **Administração**: apenas para administradores Rivier, obtendo acesso total ao painel de controle da loja, sendo possível criar/atualizar/automatizar/excluir/enviar/alterar qualquer elemento relacionado ao catálogo, além do controle de todas as informações e ações dos usuários dentro do website.

Ademais, logo abaixo temos alguns aspectos gerais de desempenho:

- O software auxila na venda da Rivier Alianças;

- Proporciona à loja maior visibilidade;

- Abrange o catálogo inteiro da empresa, possibilitando assim, de forma mais objetiva, a compra realizada pelo usuário seu produto no próprio site, de forma segura; 

- Além disso, a aplicação contribui para administração pessoal da empresa, proporcionado controle mais eficaz sobre o estoque, a renda, os gastos e as perdas financeiras (através de um painel de controle);

<br/>

## <div align="center"> 2. Desenvolvimento</div>

Por certo, todos os membros do grupo tiveram sua funções e deveres, portanto, agora serão expostas as principais tarefas, mecanismos/ferramentas utilizadas por mim, que contribuiram para o desenvolvimento dessa aplicação. Nesse trajeto, além de liderar o grupo, também efetivei encargos que envolviam back-end e front-end.


### I. Prototipação

No 2° Bimestre, a equipe teve que criar um protótipo para Pamela, no intuito de simular como seria a primeira versão do projeto, a partir do estudo de requisitos dela. Imediatamente, lembrei do editor Figma (perfeito para a prototipagem), e por conseguinte fizemos o seu uso.


<image height="340" src="https://user-images.githubusercontent.com/83969467/163688070-7574e2c1-6f1c-424b-9e41-346bd33d4e14.png" alt="Primeira tela do protótipo" title="Primeira tela do protótipo" />

> _Tela principal do protótipo_

Caso queira testar o protótipo, [**clique aqui**](https://www.figma.com/proto/MujR7rpWENjGtBm7raFwq0/Prot%C3%B3tipo---RivieraAlian%C3%A7as?node-id=1%3A2&scaling=scale-down&page-id=0%3A1&starting-point-node-id=1%3A2) para acessá-lo, você será redirecionado diretamente ao emulador do Figma.
Se por ventura o carregamento do emulador demorar, vá para [*Referências*](#4-referências), e clique no link ***Protótipo Rivier - Editor Figma***.

O design arredondado, as telas limpas com poucos elementos agrupados, a paleta de cores, a tipografia, tudo pensado e criado de acordo com o que a cliente ordenou, e logo após, era preciso decidirmos quais ferramentas faríamos o uso para o desenvolvimento.

### II. Sistema

A partir das dicas e conselhos dados por Quaiati (professor de Planejamento do Trabalho de Conclusão de Curso), conhecemos o [OpenCart](https://www.opencartbrasil.com.br/) - comércio eletrônico open source - que com certeza foi a melhor descoberta, visto que, é um sistema baseado em PHP, linguagem na qual, tive bastante experiência acadêmica.

<image height="90" src="https://user-images.githubusercontent.com/83969467/164107884-0bc36217-2830-4da4-9a69-a7fb9d20328e.png" alt="Logotipo do Open cart" title="Logotipo do OpenCart" />

> (Logotipo Open Cart)



O Opencart disponibiliza uma imensa quantidade de funções, e isso gerou bastante dificuldade para alterações no sistema, pois a arquitetura de projeto é complexa. Lidei com muitos bugs de diversas versões, mas graças às comunidades do Opencart e outros documetos pela internet, encontrei uma versão estável.

Desse modo, pude mudar toda a parte da administração e principalmente do catálogo - programado em PHP - de tal forma que o design e layout padrão concedido pelo OpenCart fosse alterado para o modelo Rivier Alianças.


### III. Linguagens

Para realizar testes e modificações, tive que fazer o uso do conhecimento de algumas linguagens para passar por esses "desafios" do sistema OpenCart, sendo elas linguagens de programação, marcação ou estilo:

<details> 
   <summary><b>PHP & Twig ...</b></summary>

   <br/>

   Além de praticamente todo o código fonte se basear em PHP, o sistema usa um mecanismo bastante produtivo que facilita absurdamente o desenvolvimento nessa linguagem, estou falando do [**Twig**](https://www.treinaweb.com.br/blog/o-que-e-twig) (um dos [*template engines*](https://www.treinaweb.com.br/blog/o-que-e-template-engine/) do php). <br/><br/> Eu nunca tinha nem ouvido falar no Twig antes, até estudar a arquitetura de pastas do OpenCart, visto que, fui capaz de perceber a importância de seu uso, porque através dele consegui manipular desde os elementos visíveis em tela, até à lógica de programação.
</details> 
<image height="88" src="https://user-images.githubusercontent.com/83969467/164113877-5ef8d5b2-705d-44a7-8617-0d87aefd979f.png" alt="Logotipo do PHP" title="Logotipo do PHP" /><image height="88" src="https://user-images.githubusercontent.com/83969467/164131862-5e154351-9bf6-493c-adcd-5d93e2168313.png" alt="Logotipo do Twig" title="Logotipo do Twig" /> 

> _Logotipo PHP - Logotipo Twig_

***

<details> 
   <summary><b> HTML & CSS ... </b></summary>

   <br/>

   Sem essas duas linguagens, seria praticamente impossível haver outra forma de renderizar e estilizar as páginas de uma maneira tão simples, uma vez que tive a capacidade de importar bibliotecas e minhas próprias estilizações à um documento php contendo diretrizes html. 
</details>



<image height="110px" src="https://user-images.githubusercontent.com/83969467/164114173-16f2c747-6a55-428c-930a-e16cb6061f55.png" alt="Logotipo do HTML" title="Logotipo do HTML" /><image height="110px" src="https://user-images.githubusercontent.com/83969467/164114069-edb22d60-f01d-4336-b223-7e3987e2316f.png" alt="Logotipo do CSS" title="Logotipo do CSS" />

>   _Logotipo HTML - Logotipo CSS_

***

<details> 
   <summary><b> MySql ... </b></summary>

   <br/>

   Utilizei conhecimentos em MySql somente para executar testes de segurança e manutenção, como por exemplo analizar se o sistema OpenCart criptografa as senhas dos usuários/administradores, ou se atualiza os dados dos produtos e usuários. <br/><br/> Cheguei à encontrar erros de atualização de hora e data, de determinadas ações feitas por clientes em simulação, tal como a finalização de um pedido. A falha aparecia no painel de controle, na parte de exibição de status dos clientes, onde a hora e data exibida estava errada. Para solucionar o problema, tive que realizar ajustes no fuso-horário pelo painel de controle, e cálculos no código da fonte dessa configuração.
</details>

<image height="92" src="https://user-images.githubusercontent.com/83969467/164113387-886db842-200f-4bdd-85e7-06ad6bf5b0ae.png" alt="Logotipo do Open cart" title="Logotipo do MySql" /> 

> _Logotipo MySql_)

***

<details> 
   <summary><b> Javascript ... </b></summary>

   <br/>

   Queria ter feito muito com esta linguagem dentro desse sistema tão grande, no entanto, consegui implementar animações, interações e acessibilidade com o **JS**, buscando oferecer ao usuário uma melhor experiência de uso.
</details>

<image height="110" src="https://user-images.githubusercontent.com/83969467/164113706-8b42d7c0-6f0d-4457-a541-55c37956c19c.png" alt="Logotipo do Open cart" title="Logotipo do Javascript" /> 

> _Logotipo Javascript_

<br/>


### IV. Servidores e CI/CD

Como o trabalho foi projetado para uma cliente real, designado à oferecer um sistema totalmente funcional *end-to-end* (de ponta à ponta), então, ele deveria ter seu próprio endereço URL para ser acessado por buscas em rede TCP/IP. Assim sendo, essa missão foi dividida em **duas** fases:

- **Fase de desenvolvimento/testes:**
   - **XAMPP** - Antes de ser lançado em produção, primeiro foi preciso testar o e-commerce em uma rede local: a opção mais cabível para um ambiente de desenvolvimento, foi [**XAMPP**](https://www.apachefriends.org/index.html), por conter um SGBD MySql, suporte à PHP, e outros pacotes de servidores, em virtude do sistema OpenCart utilizar estas mesmas ferramentas para seu controle. 

      <image height="120" src="https://user-images.githubusercontent.com/83969467/164741189-8b2396b8-a84c-4656-a089-a56dc5706bd5.png" alt="Logotipo do XAMPP" title="Logotipo do XAMPP" />

      > (Logotipo XAMPP)

   - **Netlify, Gihub.io, e InfinityFree** - Para evoluir e ao mesmo tempo não sair da fase de testes, busquei hospedar o comércio-eletrônico numa plataforma gratuita, chamada [**Netlify**](https://www.netlify.com/), a melhor que conheço até hoje, porém não obtive sucesso com ela, devido ser limitada para softwares que contenham o back-end dependente do php. <br/><br/> Similarmente, essa situação também se ocorreu após a utilização do [**Github.io**](https://pages.github.com/). <br/><br/> Eu ainda tinha um último caminho, [**InfinityFree**](https://www.infinityfree.net/). Por ser focado em hospedagem compatível com PHP e MySql, era perfeito para mostrar como a aplicação web se comportaria num ambiente online, permitindo conexões efetuadas por com qualquer pessoa. No início tudo ocorria bem, entretanto, a performance do servidor foi caindo a cada vez que era usado, gerando demora de atualização da página da loja em produção (após modificações realizadas na própria plataforma), ações lentas como upload/download/exclusão de arquivos no gerenciador de pastas, e lentidões nas tarefas do cliente-servidor.
   

      <image height="96" src="https://user-images.githubusercontent.com/83969467/164740976-577fd805-a275-4024-980c-634ee52cb72f.png" alt="Logotipo do Netlify" title="Logotipo do Netlify" /><image height="96" src="https://user-images.githubusercontent.com/83969467/164743490-afc0e525-3ace-46e6-ab0d-9286203f09e4.png" alt="Logotipo do Github.io" title="Logotipo do Github.io" /><image height="96" src="https://user-images.githubusercontent.com/83969467/164741991-eebcdb3b-c96a-4146-ae45-1c5a5e0417cb.png" alt="Logotipo do InfinityFree" title="Logotipo do InfinityFree" />

      > _Logotipos: Netlify - Github.io - InifinityFree_ 

   - **Remote MySQL** - o banco de dados do [**Remote MySQL**](https://remotemysql.com/) serviu como suporte à segurança aos dados da loja virtual - durante o desenvolvimento - pois garantia seu backup completo, portanto, o sistema teria a capacidade de conter diferentes versões de bancos, armazenados num único servidor.

- **Fase de produção:**
   - **Hostinger** - Finalmente, a loja adquiriu seu próprio domínio registrado, sendo hospedada dentro do provedor [**Hostinger**](https://www.hostinger.com.br/), obtendo o melhor desempenho na aplicação, seja no desenvolvimento ou uso. A plataforma ofereceu um ótimo gerenciamento de projeto, sem apresentar nenhum tipo de falha.

      <image src="https://user-images.githubusercontent.com/83969467/164742207-30137229-2b2d-4ce2-a671-3d8fd8e3dc1d.png" alt="Logotipo do Hostinger" title="Logotipo do Hostinger" />

      > (Logotipo Hostinger)

   - **FileZilla e Github Actions** - Para o manuseio de conexões *client/server*, primeiramente foi instalado [**FileZilla**](https://filezilla-project.org/) em minha máquina, devido o mesmo, oferecer um servidor FTP (ambiente virtual gerenciável) com um excelente funcionamento. <br/><br/> Posteriormente, descobri uma forma mais rápida e prática de estabelecer conexões FTP, tornando os workflows (fluxos de trabalho) mais rápidos, através do [**Github Actions**](https://github.com/features/actions). Com ele, foi possível realizar as práticas combinadas de **integração contínua** e **entrega contínua (CI/CD)**.

      <image height="120" src="https://user-images.githubusercontent.com/83969467/164741563-1eee2eb1-4dca-40ef-a4ba-0e053d1d65db.png" alt="Logotipo do FileZilla" title="Logotipo do FileZilla" /><image height="120" src="https://user-images.githubusercontent.com/83969467/164743294-4fceb418-a14b-4814-9200-e12d8aebd67b.png" alt="Logotipo do Actions" title="Logotipo do Actions" />
      
      > _Logotipo FileZilla - Logotipo Github Actions_


### V. Perfomance e API's

Para que o projeto e-commerce exercesse uma boa **performance** na realização de suas tarefas, seja na sua velocidade de carregamento, inicialização e processamento, ferramentas como o SASS e Gulp Js foram inseridas nesse meio. 

Por outro lado, a inserção de API's no sistema adicionou novas funções de bastante utilidade para os compradores e usuários em geral.

- ***Performance:*** 
   - [**SASS**](https://sass-lang.com/) -  a estilização foi completamente desenvolvida com um pré-processador. Dessa forma, como seu cargo é atuar como uma extensão do CSS, a administração da arquitetura de pastas da linguagem nativa foi otimizada, acelerando todo o processo de estilo.

      <image src="https://user-images.githubusercontent.com/83969467/164732331-77904f60-0ec9-4bf9-b091-1d5e7f53d875.png" alt="Logotipo do SASS" title="Logotipo do SASS" />

      > _Logotipo SASS_
   
   - [**Gulp Js**](https://gulpjs.com/) - Dentro do ambiente de desenvolvimento, fiz o uso do Gulp para automatizar tarefas como a compilação de imagens e minificação/compactação de códigos, pois ambas tarefas são um peso para a performance de uma aplicação. <br/> Pelo do sitema do projeto ser baseado em php, e o Gulp atuar como um "instrumento de automação javascript", me limitou de desfrutar mais de suas funcionalidades, como a criação/organização automatizada de pastas e arquivos, integração ao SASS, conversão de códigos, entre outros.

      <image src="https://user-images.githubusercontent.com/83969467/164732615-6e588ca1-0d9b-4ebd-b1a1-f4da76f634fe.png" alt="Logotipo do GULP JS" title="Logotipo do GULP JS" />
      
- ***API's:***
   - [**Melhor Envio**](https://melhorenvio.com.br/) - Outra implementação ao projeto foi uma API que faz a gestão de fretes, integrada à transportadoras brasileiras inclusive, que, certamente deixou a loja mais completa com este serviço à disposição.

      <image src="https://user-images.githubusercontent.com/83969467/164782161-e9968436-6a8c-4a3c-945f-05b850f0e944.png" alt="Logotipo do Melhor Envio" title="Logotipo do Melhor Envio" />

      > _Logotipo Melhor Envio_

   - **Outras API's** - outras interfaces incluídas foram: 
      - **mapa de vendas Brasil:** (exibe a quantidade de pedidos e preço total em cada estado); 
      
      - **autocomplete adress** (após o usuário inserir seu CEP para o cadastramento de conta, os campos referentes ao endereço serão preenchidos automaticamente);

      - **Validação CPF/CNPJ;**

      - **Mercado Pago;**


<br/>

## <div align="center"> 3. Documentação</div>

Para obter acesso à documentação completa do projeto, basta clicar no link de download abaixo:

[Clique aqui para baixar o PDF :page_facing_up:](https://github.com/Sancruz-dev/ecommerce-tcc-etec/files/8496832/TCC.-.DOCUMENTACAO.-.GRUPO.1.-.3DSA.pdf)

<image height="280"  src="https://user-images.githubusercontent.com/83969467/163594918-53caf93a-557d-4316-8986-b7f0675f7c5b.png" alt="Pré-visual da documentação" title="Capa da documentação" /> 

> _Pré-visual da documentação_

<br/>


## <div align="center"> 4. Referências</div>

- [Github do projeto](https://github.com/Rivier-Team/RivierAliancasOficial)
- [E-commerce Rivier Alianças](https://github.com/Rivier-Team/RivierAliancasOficial) 
- [Protótipo Rivier - Editor Figma](https://www.figma.com/file/MujR7rpWENjGtBm7raFwq0/Prot%C3%B3tipo---RivieraAlian%C3%A7as?node-id=1%3A2)




