---
author: "Valdir Ruggeri"
title: "Arquitetura REST"
date: 2022-12-27T19:30:20-03:00
description: Arquitetura REST
---
## 
A transferência de estado representacional (representational state transfer - REST) é um estilo de arquitetura de software, proposto por <a class="is-external-link" href="https://en.wikipedia.org/wiki/Roy_Fielding">Roy Thomas Fielding</a> em sua <a class="is-external-link" href="https://www.ics.uci.edu/~fielding/pubs/dissertation/fielding_dissertation.pdf">dissertação de PhD</a>, em meados de 2000. A REST foi criada inicialmente como uma diretriz para gerenciar a comunicação em uma rede complexa como a internet, possibilitando uma comunicação confiável e de alta performance em escala. Os cinco mais importantes pilares da diretriz são:



> ### Cliente-Servidor
>A comunicação ocorre entre **dois agentes**, onde um agente é considerado cliente e outro é considerado servidor. O cliente, ativamente, faz requisições que devem ser respondidas pelo servidor.

> ### Cache
>Utilizado para melhorar a performance de comunicação entre aplicações, otimizando o tempo de resposta na comunicação entre cliente-servidor.

> ### Stateless
> A comunicação entre cliente-servidor deve ocorrer independente de estado, não cabendo ao servidor      armazenar qualquer tipo de contexto, ou seja, cada requisição deve possuir toda informação necessária  >para que seja inteiramente compreensível.

> ### Camadas
> A comunicação entre cliente e servidor deve ocorrer através de camadas, onde cada camadas pode ter sua  responsabilidade, por exemplo: caching para melhorar a performance do sistema.

> ### Interface Uniforme
> Representa uma interação uniforme entre cliente e servidor. Para isso, é preciso ter uma interface que identifique e represente recursos, mensagens auto descritivas, bem como hypermedia (HATEOAS).

> ### Código sob demanda (opcional)
> A capacidade de enviar um código executável do servidor para o cliente quando solicitado para ampliar a funcionalidade disponível ao cliente.

### **REST e RESTful é a mesma coisa**

Em termos de nomenclatura, é importante sabermos a diferença entre os conceitos de REST e RESTful, como mencionado anteriormente, REST é uma diretriz composta por um conjunto de princípios e restrições de arquitetura de softwares. 

Uma API RESTful é aquela que está em conformidade com os cinco pilares que compõe a diretiva da arquitetura (REST).

Assim, quando uma API é do tipo RESTful, significa que esse sistema consegue aplicar os princípios propostos por Roy Fielding em sua tese REST.

### **Quais são os benefícios das APIs RESTful?**

**Escalabilidade**  
Os sistemas que implementam APIs REST podem ser escalados com eficiência, porque a REST otimiza as interações entre cliente e servidor. A ausência de estado remove a carga do servidor, porque o servidor não precisa reter informações de solicitações anteriores do cliente. O cache bem gerenciado elimina parcial ou completamente algumas interações entre cliente e servidor. Todos esses recursos permitem a escalabilidade sem causar gargalos de comunicação que reduzem a performance.

**Flexibilidade**  
Os serviços da Web RESTful permitem a separação total do cliente do servidor. Eles simplificam e desacoplam vários componentes do servidor para que cada parte possa evoluir independentemente. Mudanças de plataforma ou tecnologia na aplicação do servidor não afetam a aplicação do cliente. 

**Independência**  
APIs REST são independentes da tecnologia usada. Você pode escrever aplicações de cliente e servidor em várias linguagens de programação sem afetar o design da API. Também é possível alterar a tecnologia subjacente em ambos os lados sem afetar a comunicação.