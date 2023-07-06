# AWS-SiteEstaticoTCC

**PROJETO WEBSITE PARA DIVULGAÇÃO DE CURRÍCULOS** <br>
Desenvolvimento de um website (html, css, imagens) contendo os currículos do grupo e a implantação de um ou mais serviços na nuvem AWS, com rede de entrega de conteúdo, com baixa latência, com segurança, e armazenamento durável, para atender a demanda de 11 milhões de requisições por mês.<br>
<br>
**GRUPO 01**<br>
Alanis Cristina Ribeiro Silva<br>
Akyssa Eduarda<br>
Alinyy Ribeiro<br>
Darwin Giovanni<br>
Diogo da Silva<br>
<br>
**Mentor**<br>
Rodolfo dos Santos Silva<br>
<br>
**SERVIÇOS UTILIZADOS**<br>
**Amazon S3** (Armazenamento escalável, duradouro e seguro) – Armazena os arquivos HTML, CSS, Javascript e Imagens; escalabilidade; integração com Cloudfront e durabilidade dos objetos armazenados.<br>
<br>
**Amazon CloudFront** (Entrega de conteúdo por meio de uma rede global de servidores) – Melhora o desempenho e escalabilidade do site; melhora a velocidade de entrega e fornece recursos de segurança.<br>
<br>
**ARQUITETURA DO PROJETO**<br>
<br>
![2023-07-05](https://github.com/alanisribeiro/AWS-SiteEstaticoTCC/assets/126534588/f736358a-6477-43fe-946d-dca7b5908447)<br>
<br>
**EXPLICANDO A ARQUITETURA**<br>
**1.** O usuário faz uma solicitação para acessar o site estático<br>
**2.** O CloudFront recebe a solicitação do usuário e verificar se o conteúdo está disponível no ponto de acesso mais próximo<br>
(Se não estiver disponível o Cloudfront vai até o S3, busca os arquivos e devolve para o usuário final)<br>
**3.** Se o conteúdo estiver em cache no ponto de acesso mais próximo do usuário, o CloudFront o entrega e dá uma resposta de baixa latência<br>
**4.** O S3 entrega o arquivo solicitado pelo CloudFront<br>
**5.** O CloudFront armazena o arquivo em cache no ponto de presença<br>
**6.** O CloudFront entrega o arquivo solicitado pelo usuário, fornecendo uma resposta rápida e de baixa latência<br>
**7.** E o usuário recebe o recurso solicitado e consegue visualizar o site estático


**CUSTO**<br>
Mental - 6,20 USD<br>
Custo total por 12 meses - 74,40 USD.




