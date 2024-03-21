# Data Transfer Object (TDO)

Padrão de software voltado para a transferência de dados entre as camadas de uma aplicação. Ele consiste basicamente no entendimento de como as informações trafegam dentro de um sistema. 

Quando desenvolvemos uma aplicação existem diversas responsabilidades e camadas que separam detalhes, como: o coração da aplicação, o seu comportamento, as comunicações e como os dados externos são recebidos.

---

## Compatibilidade

A questão é que dados externos podem vir de diversas maneiras e formatos, como API REST, CLI, gRPC ou sistemas de mensageria. E como os dados não necessariamente chegam num formato compatível, as informações passam pelas camadas mais internas do sistema até chegarem ao nível de entidade, que são os fundamentos básicos de toda a aplicação. 

Pensando nesses detalhes nós podemos criar um objeto, que é basicamente uma classe, dependendo do contexto no qual você está inserido. Mas a ideia é que você tenha um objeto totalmente anêmico, que vai apenas receber os dados naquele estado específico. Ele vai, por exemplo, fazer a serialização de JSON ou XML, preenchendo a sua propriedade exatamente num formato que a sua entidade, caso de uso ou seu serviço precisa receber, sem fazer qualquer contato entre as camadas inferiores do seu sistema.

Com o serviço preparado para receber o seu dado num determinado formato, o DTO pega as informações, processa, chama entidades e pode rodar as suas regras de negócio para te retornar com um resultado.

---
# Analogia 

DTO é como se fosse uma sacola de compras de supermercado. O supermercado seria o fornecedor de "dados" que seriam os itens da compra. Você não compra tudo do supermercado, logo, você diz para a sacola (DTO) só o que você precisa ter. Uma vez na sacola você não mexe nelas até chegar em casa (camada de domínio).