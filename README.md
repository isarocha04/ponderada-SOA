# ponderada-SOA

1 - Para atender as necessidades da companhia aérea de desenvolver um sistema de reservas de voos altamente integrado e capaz de proporcionar uma experiência de usuário de alta qualidade, uma possível arquitetura SOA simples seria constituída dos seguintes blocos principais:

Camada de Interface do Usuário (UI): Essencial para a interação direta dos clientes com o sistema, essa camada permite a pesquisa, seleção e reserva de voos, bem como o cadastro de novos usuários. Uma interface amigável e responsiva é essencial para uma experiência positiva do usuário.

Camada de Lógica de Negócios: Centraliza o processamento de regras de negócios específicas da companhia aérea, como validações de reservas, cálculos de preços e políticas de cancelamento. Isolando a lógica de negócios, essa camada promove a modularidade e facilita atualizações e manutenções.

Camada de Serviços SOA Externos: Integração de APIs de terceiros para enriquecer o sistema com funcionalidades adicionais, como serviços de pagamento, informações meteorológicas para destinos de voos e geolocalização para detectar a localização atual do usuário. A escolha de parceiros confiáveis e a gestão eficiente de APIs são críticas para a expansão das capacidades do sistema sem comprometer o desempenho.

Camada de Acesso a Dados: Gerencia a persistência e recuperação de dados relacionados a voos, reservas, e perfis de usuário. A separação da lógica de negócios do acesso aos dados permite flexibilidade na escolha de bancos de dados e otimiza o desempenho das consultas.

Diagrama Conceitual da Arquitetura:

![image](https://github.com/isarocha04/ponderada-SOA/assets/99424901/50bbbd39-4ed8-4429-8262-1e9b712c1213)

 - Interface do Usuário (UI): Permite a interação dos usuários com o sistema, abrangendo a pesquisa, seleção, e reserva de voos.
 - Lógica de Negócios: Centraliza o processamento das regras de negócios da companhia aérea, facilitando a modularidade e a manutenção.
 - Serviços SOA Externos: Integra funcionalidades adicionais por meio da integração com APIs de terceiros.
 - Camada de Acesso a Dados: Gerencia os dados relacionados a voos, reservas, e perfis de usuários, conectando-se ao Banco de Dados.

2 -  Requisitos Não Funcionais Detalhados
Elasticidade para Lidar com Picos de Demanda: O sistema deve ser capaz de automaticamente escalar recursos de infraestrutura, como aumentar o número de servidores, para lidar com aumentos na demanda sem degradar a performance. Isso é essencial para manter a alta disponibilidade e a satisfação do usuário, especialmente durante períodos de alta demanda, como feriados e promoções.

Performance (Tempo Máximo de Resposta): O sistema deve garantir tempos de resposta rápidos para pesquisas de voos e transações de reserva, melhorando assim a experiência do usuário. A definição de métricas de performance claras, como tempos de resposta máximos para cada tipo de requisição, é crucial para medir e otimizar a eficiência do sistema.

Disponibilidade Contínua: O design do sistema deve assegurar uma alta disponibilidade, utilizando técnicas como redundância, failover e balanceamento de carga. A capacidade de manter o sistema operacional mesmo em face de falhas de componentes individuais é fundamental para a confiabilidade e a reputação da companhia aérea.

Segurança de Dados Sensíveis: Implementação de rigorosos controles de segurança para proteger dados sensíveis dos usuários, como informações pessoais e de pagamento. Isso inclui criptografia de dados, autenticação segura e conformidade com padrões internacionais de segurança. A arquitetura SOA deve promover a implementação consistente de políticas de segurança em todos os serviços.

Testabilidade e Monitoramento: A infraestrutura deve suportar a testabilidade contínua e o monitoramento em tempo real dos serviços para garantir a detecção e correção rápida de problemas. A separação de serviços facilita a implementação de testes automatizados e monitoramento detalhado, essenciais para a manutenção da qualidade e a identificação precoce de problemas.
