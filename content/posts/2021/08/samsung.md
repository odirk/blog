---
title: "Bloqueando propagandas em Smart TVs"
date: "2021-08-24"
tags: ["tech"]
description: "I'm sorry, Dave. I'm afraid I can't do that."
draft: false
---

Estou com uma tv nova da Samsung há uns meses e percebi que existem anúncios da Samsung na barra de input (aquela em que você escolhe a fonte de entrada ou acessa apps). Então, decidi fazer algo a respeito.

{{< figure align=center src="/samsung/ad.jpg" title="Enfurecedor, não é?" >}}

Minha primeira resposta foi de total indiganação, como a Samsung pode exibir anúncios na minha TV sem o meu consentimento? Eu paguei o preço pela TV e eles não têm o direito de fazer nada na TV.

{{< youtube RfprRZQxWps >}}
> Fucking double dippers, Jerry!

Eu até verifiquei se é possível formatar o sistema operacional da TV e instalar algo de código aberto mais orientado para privacidade, mas essa opção parecia tediosa e exigiu mais tempo.

Mas, para minha surpresa, bloquear anúncios na sua smart foi muito simples. Basta filtrar um monte de domínios ou alterar o DNS no seu roteador de internet. Para fazer isso, siga as etapas abaixo:

1. Abra a página de configuração do seu roteador. Para isso, abra a página de configuração do roteador em um navegador da web em um computador/celular conectado à sua rede.

Esse endereço deve estar escrito na lateral de seu roteador (geralmente é http://192.168.0.1), junto com login e senha.

2. Localize a página sobre o DNS. (Na Claro ficam dentro das *Configurações avançadas*).

3. O [AdGuard](https://adguard.com/pt_br/adguard-dns/overview.html) possui servidores de DNS que bloqueiam propagandas na web, e eles funcionam contra as propagandas da Samsung.

Adicione os seguintes endereços na página:

| IPv4 | IPv6 |
| ---- | ---------- |
| 94.140.14.14 | 2a10:50c0::ad1:ff |
| 94.140.15.15 | 2a10:50c0::ad2:ff |

{{< figure align=center src="/samsung/claro.png" >}}

4. Clique em salvar e é só isso!

As propagandas ainda vão continuar aparecendo por alguns dias (pois estão salvas na televisão), mas todas elas deixarão de aparecer dentro de alguns dias. :tada: