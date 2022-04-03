# Fundamentos de Arquitetura de Software

- [Fundamentos de Arquitetura de Software](#fundamentos-de-arquitetura-de-software)
  - [Fundamentos](#fundamentos)
    - [Aula 01 - Arquitetura tecnológica e corporativa](#aula-01---arquitetura-tecnológica-e-corporativa)
      - [Tipos de Arquitetura](#tipos-de-arquitetura)
      - [Arquitetura Tecnológica](#arquitetura-tecnológica)
      - [Arquitetura Corporativa](#arquitetura-corporativa)
    - [Aula 02 - Arquitetura de solução](#aula-02---arquitetura-de-solução)
      - [Arquitetura de solução](#arquitetura-de-solução)
    - [Aula 03 - Arquitetura de software](#aula-03---arquitetura-de-software)
      - [Arquiteto de software](#arquiteto-de-software)
    - [Aula 04 - O papel do arquiteto de software](#aula-04---o-papel-do-arquiteto-de-software)
    - [Aula 05 - Por que aprender arquitetura de software?](#aula-05---por-que-aprender-arquitetura-de-software)
    - [Aula 06 - Arquitetura vs Design](#aula-06---arquitetura-vs-design)
    - [Aula 07 - Sustentabilidade no dia zero](#aula-07---sustentabilidade-no-dia-zero)
    - [Aula 08 - Pilares da arquitetura de software](#aula-08---pilares-da-arquitetura-de-software)
    - [Aula 09 - Requisitos arquiteturais (RAs)](#aula-09---requisitos-arquiteturais-ras)
  - [Caracteristícas Arquiteturais](#caracteristícas-arquiteturais)
    - [Caracteristícas operacionais](#caracteristícas-operacionais)
    - [Caracteristícas estruturais](#caracteristícas-estruturais)
    - [Cross-Cutting](#cross-cutting)
  - [Performance](#performance)
    - [Perspectivas para arquitetar software de qualidade](#perspectivas-para-arquitetar-software-de-qualidade)
    - [Métricas para medir performance](#métricas-para-medir-performance)
      - [Como melhorar a performance?](#como-melhorar-a-performance)
      - [Principais razões para a baixa performance](#principais-razões-para-a-baixa-performance)
      - [Principais formas para aumentar a eficiência](#principais-formas-para-aumentar-a-eficiência)
    - [Capacidade computacional: Escala vertical vs Escala horizontal](#capacidade-computacional-escala-vertical-vs-escala-horizontal)
      - [Escala vertical](#escala-vertical)
      - [Escala horizontal](#escala-horizontal)
      - [Diferenças entre concorrência e paralelismo](#diferenças-entre-concorrência-e-paralelismo)
    - [Caching](#caching)
      - [Caching Exclusivo vs Compartilhado](#caching-exclusivo-vs-compartilhado)
    - [Caching vs Edge Computing](#caching-vs-edge-computing)
      - [Edge Computing](#edge-computing)
  - [Escalabilidade](#escalabilidade)
    - [Escalabilidade vs Performance](#escalabilidade-vs-performance)
    - [Escalando aplicações](#escalando-aplicações)
    - [Escala de banco de dados](#escala-de-banco-de-dados)
    - [Proxy reverso](#proxy-reverso)

## Fundamentos

### Aula 01 - Arquitetura tecnológica e corporativa

#### Tipos de Arquitetura

- Software
- Solução
- Tecnológica
- Corporativa

#### Arquitetura Tecnológica

- Especialidade em tecnologias específicas de mercado
- Geração de valor baseado em especialidades
- Diversidade de processionais especialistas. Exemplos:
  - Arquiteto Elastic
  - Arquiteto Java
  - Arquiteto AWS
  - Arquiteto SQL Server

#### Arquitetura Corporativa

- Impacta estrategicamente a organização como um todo
- Avaliação de custos
- Avaliação de possíveis novas tecnologias
- Padronização de tecnologias
- Planejamento de grandes implantações
  - Sistemas "core"
  - Migrações

### Aula 02 - Arquitetura de solução

#### Arquitetura de solução

- Fica entre a área de negócios e software
- Transforma requisitos de negócio em soluções de software
- Desenhos arquiteturais da solução de um software para reproduzir como ele irá funcionar
  - C4
  - UML
  - BPMN
- Analisa os impactos comerciais em relação a uma escolha tecnológica
- Pode participar do processo comercial de pré-venda e venda
- Analisa os impactos dos custos para o negócio

### Aula 03 - Arquitetura de software

#### Arquiteto de software

É a relação entre os objetivos de negócios e suas restrições com os componentes a serem criados e suas responsabilidades visando a evolução do software.

"É a organização fundamental de um sistema e seus componentes, suas relações, seu ambiente, bem como os princípios que guiam seu design e evolução." (IEEE Standard 1471).

- É uma disciplina da Engenharia de Software
- Diretamente ligada ao processo de desenvolvimento de software
- Afeta diretamente na estrutura organizacional da empresa
  - Formação dos times
  - Estrutura dos componentes do software
  - "Organizações que desenvolvem sistemas de software tendem a produzir sistemas que são cópias das estruturas de comunicação dessas empresas." (Melvin Conway)

O processo de arquitetar um software estabelece que o que está sendo desenvolvido faça parte de um conjunto maior.

### Aula 04 - O papel do arquiteto de software

- Transformar requisitos de negócio em padrões arquiteturais
- Orquestrar pessoas desenvolvedores e experts de domínio
- Entender de forma profunda conceitos e modelos arquiteturais
- Auxilia na tomada de decisão nos momentos de crise
- Reforça boas práticas de desenvolvimento
- Faz Code reviews

Apesar de nem todas as organizações possuírem o cargo de arquiteto de software, normalmente profissionais mais experientes como desenvolvedores seniores e tech leads acabam realizando esse papel baseado em suas experiências anteriores.

Há empresas que apesar de não possuírem o cargo de Arquiteto de Software, possuem um departamento de arquitetura que auxilia os diversos times da organização com questões arquiteturais.
Sustentabilidade no dia zero

### Aula 05 - Por que aprender arquitetura de software?

- Pode navegar da visão macro para a visão micro de um ou mais softwares
- Entender quais são as diversas opções que temos para desenvolver a mesma coisa e escolher a melhor solução para determinado contexto
- Pensar a longo prazo no projeto e sua sustentabilidade
- Tomar decisões de forma mais fria e calculada evitando assim ser influenciado por hypes de mercado
- Mergulho em padrões de projetos e de desenvolvimento e suas boas práticas
- Ter mais clareza do impacto que o software possui na organização como um todo
- Tomar decisões com mais confiança

### Aula 06 - Arquitetura vs Design

"Atividades relacionadas a arquitetura de software são sempre de design. Entretanto, nem todas as atividades de design são sobre arquitetura. O objetivo primário da arquitetura de software é garantir que os atributos de qualidade, restrições de alto nível e os objetivos do negócio, sejam atendidos pelo sistema. Qualquer decisão de design que não tenha relação com este objetivo não é arquitetural. Todas as decisões de design para um componente que não sejam visíveis fora dele, geralmente, também não são." (Elemar Jr.)

- Arquitetura: Escopo global ou alto nível
- Design: Escopo local

### Aula 07 - Sustentabilidade no dia zero

### Aula 08 - Pilares da arquitetura de software

- Estruturação
  - Fácil evolução, componentização para atender os objetivos de negócios
- Componentização
- Relacionamento entre sistemas
- Governança (padronização, regras, documentação)

### Aula 09 - Requisitos arquiteturais (RAs)

- Performance
- Armazenamento de dados
- Escalabilidade
- Segurança
- Legal (legislação)
- Auditoria
- Marketing

## Caracteristícas Arquiteturais

Trabalhar pontos arquiteturais de forma intencional.

### Caracteristícas operacionais

- Disponibilidade
- Recuperação de desastres
- Performance
- Recuperação (backup)
  - Testar Backup
- Confiabilidade e segurança
- Robustez
- Escalabilidade
  - Escala vertical (aumentar recursos)
  - Horizontal (adicionar instâncias)

### Caracteristícas estruturais

- O software precisa ser configurável
- A aplicação precisa ser extensível, de modo que outras coisas possam ser plugáveis nela
  - Não deve ser necessário fazer mudanças estruturais na aplicação para adicionar uma nova gateway é por que a aplicação está projetada de forma incorreta
- Fácil instalação
- Reuso de componentes
- Internacionalização
  - Valores monetários
  - Horários
- Fácil manutenção
  - Correção de bugs deve ser fácil
  - Adicionar novas features deve ser fácil
  - O sistema deve ter testes
- Portabilidade
  - diversos bancos de dados
  - gateways
- Fácil suporte
  - Foque em observabilidade
  - logs
  - debugging

### Cross-Cutting

- Acessibilidade
- Processo de retenção e recuperação de dados
  - Quanto tempo os dados serão mantidos?
- Autenticação e autorização
- Parte Legal
  - Conformidade com as leis do país que o aplicativo executa
- Privacidade
- Segurança
- Usabilidade

## Performance

### Perspectivas para arquitetar software de qualidade

- Performance
- Escalabilidade
- Resiliência

### Métricas para medir performance

- É o desempenho que um software possui para completar um determinado workload.
- As unidades de medida para avaliarmos a performance de um software são:
  - Latência ou response time
  - Throughput (quantas requisições um software aguentar receber)
- Ter um software performático é diferente de ter um software escalável

#### Como melhorar a performance?

- Diminuindo a latência
  - Normalmente medida em milliseconds
  - É afetada pelo tempo de processamento da aplicação, rede e chamadas externas
- Aumentando throughput
  - Aumentando quantidade de requisições
  - É totalmente ligado a latência
  - Diminuir a quantidade de conexões presas à aplicação

#### Principais razões para a baixa performance

- Processamento ineficiente
- Recursos computacionais limitados
- Trabalhar de forma bloqueante
- Acesso serial a recursos

#### Principais formas para aumentar a eficiência

- Escala da capacidade computacional (CPU, Disco, Memória, Rede)
- Lógica por trás do software (Algoritmos, queries, overhead de frameworks)
- Concorrência e paralelismo
- Banco de dados (tipos de bancos, schema, normalização, indices, apm)
- Caching

### Capacidade computacional: Escala vertical vs Escala horizontal

#### Escala vertical

Cada vez que preciso aumentar a capacidade de lidar com mais requisições eu aumento a capacidade computacional.

#### Escala horizontal

Ao invés de aumentar a capacidade computacional da máquina eu aumento a quantidade de máquinas.

#### Diferenças entre concorrência e paralelismo

"Concorrência é sobre lidar com muitas coisas ao mesmo tempo. Paralelismo é fazer muitas coisas ao mesmo tempo." - Rob Pike

### Caching

- Cache na borda / Edge computing
- Dados estáticos
- Páginas web
- Funções internas
  - Evitar processamento de algoritmos pesados
  - Acesso ao banco de dados
- Objetos

#### Caching Exclusivo vs Compartilhado

- Exclusivo
  - Baixa latência
  - Duplicado entre os nós
  - Problemas relacionados a sessões
- Compartilhado
  - Maior latência
  - Não há duplicação
  - Sessões compartilhadas
  - Banco de dados externo
    - MySQL
    - Redis
    - Memcache

### Caching vs Edge Computing

#### Edge Computing

Ajuda a fazer com que a informação do usuário esteja perto dele, evitando tráfego desnecessário de informações.

- Cache realizado mais próximo ao usuário
- Evita a requisição chegar até o Cloud Provider / Infra
- Normalmente arquivos estáticos
- CDN (Content Delivery Network)
- Cloudflare workers
  - Cloudflare é uma plataforma de Cache Computer.
  - Permite deploy de aplicações em locais mais próximos da localização física do usuário
- Vercel
- Akamai

## Escalabilidade

É a capacidade de sistemas suportarem o aumento, ou redução dos workloads, incrementando ou reduzindo os custos em menor ou igual proporção.

### Escalabilidade vs Performance

Enquanto performance tem o foco em reduzir a latência e aumentar o throughput, a escalabilidade visa termos a possibilidade de aumentar ou diminuir o throughput adicionando ou removendo a capacidade computacional.

### Escalando aplicações

Quando vou escalar o software horizontalmente eu vou aumentar o número de máquinas, quando diminuir o uso vou descartar essas máquinas adicionais.
As máquinas devem ser adicionadas e removidas rapidamente.

- Disco efêmero
  - Tudo que eu salvar em disco na máquina deve poder ser apagado
  - O disco deve ser utilizado para gravar arquivos temporários.
- Servidor de aplicação vs Servidor de assets
  - Devem ser servidores diferentes o local da aplicação e o local de armazenamento de imagens, etc...
- Cache centralizado
  - O cache não vai ficar na sua máquina
  - Deverá ficar em um servidor externo específico para cache
- Sessões centralizadas
  - As sessões devem estar centralizadas em um único servidor, onde as máquinas escaladas se servirão dos dados
- Upload e gravação de arquivos
  - Devem estar armazenados em um servidor de arquivos a parte

**Escalar software significa descentralizar.**

### Escala de banco de dados

- Aumentando recursos computacionais
- Distribuindo responsabilidades (escrita vs leitura)
  - Criar um banco específico para leitura e outro específico para escrita
- Shards de forma horizontal
  - Mudar o formato
  - Adicionar várias máquinas
  - Dividir partições no banco de dados
- Serverless
  - Não se preocupar a nível de servidor
- Otimização de queries e índices
  - Sistema de APM para banco de dados
  - Trabalhar com índices de forma consciente
  - Explain nas queries
  - CQRS (command Query Responsability Segregation)

### Proxy reverso

É um servidor que fica na frente dos servidores web e encaminha as solicitações do cliente, por exemplo um navegador web, para esses servidores web.
Recebe todas as requisições e baseado na requisição redistribui a solicitação para determinado servidor.
