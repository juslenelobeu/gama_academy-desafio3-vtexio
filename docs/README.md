# Desafio #3 - Gama Academy

Replicar a interface do [UpMedal](https://www.upmedal.com/desafios) aplicando VTEX IO

![screenshot](https://github.com/juslenelobeu/gama_academy-desafio-03-vtexio/blob/master/screenshot.jpeg?raw=true)

## Link do workspace desse desafio

[https://desafio3juslenelobeu--hiringcoders2021.myvtex.com](https://desafio3juslenelobeu--hiringcoders2021.myvtex.com/)

### Este projeto contém um componente de Form Lead que esta salvando os dados no localStorage e no DynamoDB AWS
Link do componente [https://github.com/juslenelobeu/store-block-template-vtex-io](https://github.com/juslenelobeu/store-block-template-vtex-io)

## Video Preview
https://youtu.be/yBDuNGQbphA
<hr>

1. Criei um **workspace** exclusivo para o desafio

```powershell
vtex use desafio3juslenelobeu
```

2. Confirmando em qual **workspace** eu estou

```powershell
vtex whoami
```

3. Iniciando um novo tema com o **boilerplate** padrão

```powershell
vtex init
```

4. Com o template baixado, entrei na pasta do tema

```powershell
cd minimum-boilerplate-theme
```

5. Alterei o arquivo `manifest.json` com o nome da account do curso **hiringcoders2021** e nome do desafio

```json
"vendor": "hiringcoders2021",
"name": "desafio-3-juslenelobeu"
```

6. Linkei o tema no workspace criado

```powershell
vtex link
```

## Tasks

1. O que precisa cumprir para esse desafio:
 - [X]  Flex layout - [https://vtex.io/docs/components/all/vtex.flex-layout@0.17.0/](https://vtex.io/docs/components/all/vtex.flex-layout@0.17.0/)
 - [X]  Criar arquivos em .jsonc para colocar os comentários de seus blocos
 - [X]  Slider layout para mostrar produtos em destaque - [https://vtex.io/docs/app/vtex.slider-layout](https://vtex.io/docs/app/vtex.slider-layout)
 - [X]  Criar componente Tab layout para separar produtos por categoria - [https://vtex.io/docs/components/all/vtex.tab-layout@0.4.3/](https://vtex.io/docs/components/all/vtex.tab-layout@0.4.3/)
 - [X]  Criar um bloco de lista de produto - [https://vtex.io/docs/app/vtex.product-list@0.31.0/](https://vtex.io/docs/app/vtex.product-list@0.31.0/)

     Sugestão paginado por 8 itens da categoria

 - [X]  Criar Minicart para lista dos produtos no carrinho - [https://vtex.io/docs/components/content-blocks/vtex.minicart@2.60.0/](https://vtex.io/docs/components/content-blocks/vtex.minicart@2.60.0/)
 - [X]  Ao clicar no produto ir para a tela com Product Summary - [https://vtex.io/docs/components/all/vtex.product-summary@2.53.0/](https://vtex.io/docs/components/all/vtex.product-summary@2.53.0/)
 - [ ]  Layout mobile
 - [ ]  Criar um componente customizado para falar com suporte no whatsapp, no rodapé
     - [ ]  Utilizar o Vtex Components com React - [https://vtex.io/docs/components/all/vtex.store-components@3.150.0/](https://vtex.io/docs/components/all/vtex.store-components@3.150.0/)
     - [ ]  API whatsapp - [https://www.convertte.com.br/gerador-link-whatsapp/](https://www.convertte.com.br/gerador-link-whatsapp/)
 - [X]  Criar um componente customizado para cadastrar leads (possíveis clientes prospectos)
 ○ Nome
 ○ Email
 ○ Telefone

## Este componente Form Lead esta salvando no localStorage e no **DynamoDB**
Link do componente [https://github.com/juslenelobeu/store-block-template-vtex-io](https://github.com/juslenelobeu/store-block-template-vtex-io)

Este componente pode servir de isca digital, fazendo dando uma bonificação para o prospecto que preencher as informações da lead.
Utilizar o Vtex Componentes com React para criar o componente - [https://vtex.io/docs/components/all/vtex.store-components@3.150.0/](https://vtex.io/docs/components/all/vtex.store-components@3.150.0/)

[https://vtex.io/docs/getting-started/desenvolva-componentes-usando-vtex-io-e-react/](https://vtex.io/docs/getting-started/desenvolva-componentes-usando-vtex-io-e-react/)

## AWS API Gateway

- [x]  Com o objetivo de armazenar as leads que o Vtex componente irá utilizar no React, criar uma API Gateway na AWS para colocar as informações - [https://aws.amazon.com/pt/api-gateway/](https://aws.amazon.com/pt/api-gateway/)
- Um exemplo de arquivo API Gateway para estudo:
- [https://github.com/awslabs/aws-api-gateway-developer-portal/blob/master/cloudformation/template.yaml](https://github.com/awslabs/aws-api-gateway-developer-portal/blob/master/cloudformation/template.yaml)
- [https://github.com/mattpodolak/email-api-lambda](https://github.com/mattpodolak/email-api-lambda)
- [https://github.com/amazon-archives/realworld-serverless-application/blob/master/backend/sam/app/api.template.yaml](https://github.com/amazon-archives/realworld-serverless-application/blob/master/backend/sam/app/api.template.yaml)
