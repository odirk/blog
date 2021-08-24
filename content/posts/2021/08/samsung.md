---
title: "Bloqueando propagandas em Smart TVs"
date: "2021-08-24"
tags: ["tech"]
description: "I'm sorry, Dave. I'm afraid I can't do that."
draft: false
---

Estou com uma TV nova da Samsung há uns meses e percebi que existem anúncios da Samsung na barra de input (aquela em que você escolhe a fonte de entrada ou acessa apps).

{{< figure align=center src="/samsung/ad.jpg" title="Enfurecedor, não é?" >}}

Minha primeira resposta foi de total indiganação, como a Samsung pode exibir anúncios na minha TV sem o meu consentimento? Eu paguei o preço por ela e eles não têm o direito de ganhar mais dinheiro de anunciantes.

&nbsp;
&nbsp;

{{< youtube RfprRZQxWps >}}
> Fucking double dippers, Jerry!

&nbsp;
&nbsp;

Eu até verifiquei se é possível formatar o sistema operacional da TV e instalar algo de código aberto mais orientado para privacidade, mas essa opção parecia tediosa e exigiu mais tempo.

Mas, para minha surpresa, bloquear anúncios na sua smart foi muito simples. Basta filtrar um monte de domínios ou alterar o DNS no seu roteador de internet. Para fazer isso, siga as etapas abaixo:

&nbsp;
&nbsp;

### 1. Acesse o router

Abra a página de configuração do seu roteador. Para isso, abra a página de configuração do roteador em um navegador da web em um computador/celular conectado à sua rede.

Esse endereço deve estar escrito na lateral de seu roteador (geralmente é [http://192.168.0.1](http://192.168.0.1)), junto com login e senha.

&nbsp;
&nbsp;

### 2. Acesse a página de DNS

Localize a página sobre o DNS. (Na Claro ficam dentro das *Configurações avançadas*).

> O [AdGuard](https://adguard.com/pt_br/adguard-dns/overview.html) possui servidores de DNS que bloqueiam propagandas na web, e eles funcionam contra as propagandas da Samsung.

Adicione os seguintes endereços na página:

| IPv4 | IPv6 |
| ---- | ---------- |
| 94.140.14.14 | 2a10:50c0::ad1:ff |
| 94.140.15.15 | 2a10:50c0::ad2:ff |

{{< figure align=center src="/samsung/claro.png" title="Assim" >}}

&nbsp;
&nbsp;

### 3. Salve as alterações

Clique em salvar e é só isso!

As propagandas ainda vão continuar aparecendo por alguns dias (pois estão salvas na televisão), mas todas **elas deixarão de aparecer em breve**. :tada: