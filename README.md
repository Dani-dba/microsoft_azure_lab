# Microsoft Azure Lab

Este repositório documenta minhas experiências e aprendizados com o Microsoft Azure, com base nas trilhas de estudos do Microsoft Docs e laboratórios práticos.

## Resumo

Iniciei os estudos utilizando uma conta gratuita do Azure, previamente criada para fins acadêmicos. Durante as aulas, explorei os principais conceitos relacionados à computação em nuvem, incluindo:

- **Tipos de nuvem**: Pública, privada e híbrida.
- **Modelos de custos**: Diferenças entre CapEx (Capital Expenditure) e OpEx (Operational Expenditure), com exemplos práticos.
- **Benefícios da nuvem**:
  - Alta disponibilidade
  - Escalabilidade
  - Elasticidade
  - Confiabilidade
  - Previsibilidade
  - Segurança
  - Governança
  - Gerenciabilidade

## Experiências Práticas

Durante o laboratório, aprendi a:
- Customizar a aparência do portal Azure.
- Navegar e localizar serviços por categorias dentro da plataforma.

## Benefícios da nuvem - Laboratório 19/09/2024 15:15
#### SLA (Service Level Agreement) e os 9's

No Azure, o SLA define o percentual de disponibilidade garantido para os serviços. A disponibilidade é medida com base no número de "9's", o que impacta diretamente o tempo de indisponibilidade permitido. Abaixo está uma tabela detalhando o tempo de inatividade máximo por nível de SLA em diferentes períodos (semana, mês e ano):

| Nível de SLA     | Disponibilidade | Tempo Máximo de Inatividade por Semana | Tempo Máximo de Inatividade por Mês | Tempo Máximo de Inatividade por Ano  |
|------------------|-----------------|----------------------------------------|-------------------------------------|--------------------------------------|
| 99%              | 99%             | 1,68 hora                              | 7,2 horas                           | 3,65 dias                            |
| 99.9%            | 99.9%           | 10,1 minutos                           | 43,2 minutos                        | 8,76 horas                           |
| 99.95%           | 99.95%          | 5 minutos                              | 21,6 minutos                        | 4,38 horas                           |
| 99.99%           | 99.99%          | 1,01 minutos                           | 4,32 minutos                        | 52,56 minutos                        |
| 99.999%          | 99.999%         | 6 segundos                             | 25,9 segundos                       | 5,26 minutos                    |

#### Zonas de Disponibilidade

A escolha da **zona de disponibilidade** é crucial para garantir alta disponibilidade e resiliência contra falhas regionais. Cada região do Azure pode ter várias zonas de disponibilidade, fisicamente separadas, para proteger contra falhas de energia, rede e hardware. É importante levar em consideração a redundância geográfica ao projetar aplicações e serviços para garantir que um incidente em uma zona não afete a operação.

#### Contas de Armazenamento

No Azure, existem diferentes tipos de **contas de armazenamento**, cada uma com sua própria precificação. A escolha do tipo de conta afeta o custo com base no desempenho e nas funcionalidades necessárias. Os principais tipos de contas são:


- **LRS (Locally Redundant Storage)**: Mantém três cópias dos dados dentro de um único datacenter na mesma região. É a opção mais econômica, mas oferece menor tolerância a falhas regionais.
- **GRS (Geo-Redundant Storage)**: Armazena três cópias localmente e mais três cópias em uma região secundária distante. Oferece maior resiliência em caso de desastres, com custo adicional.
- **ZRS (Zone-Redundant Storage)**: Replica os dados entre três zonas de disponibilidade diferentes dentro da mesma região, garantindo alta disponibilidade e proteção contra falhas de zona.
- **GZRS (Geo-Zone-Redundant Storage)**: Combina replicação entre zonas de disponibilidade e replicação geográfica, armazenando dados em várias zonas em uma região primária e em uma região secundária distante, oferecendo o nível mais alto de resiliência e disponibilidade.

A escolha do tipo de conta depende dos requisitos de disponibilidade, desempenho e custo do projeto.

#21/09/2024
## Tipos de Serviço em Nuvem: IaaS, PaaS e SaaS

Na última aula, foram explorados os principais modelos de serviço em nuvem: 
- **IaaS (Infrastructure as a Service)**
- **PaaS (Platform as a Service)**
- **SaaS (Software as a Service)**.

Cada modelo oferece diferentes níveis de gerenciamento e responsabilidade, conforme descrito abaixo:
- **IaaS (Infrastructure as a Service)**: Proporciona recursos de computação em nuvem, como servidores virtuais, armazenamento e redes. O usuário é responsável pela instalação e gerenciamento do sistema operacional e dos aplicativos, enquanto o provedor cuida da infraestrutura física.

- **PaaS (Platform as a Service)**: Oferece uma plataforma completa para desenvolvimento, testes e implantação de aplicações. O provedor gerencia a infraestrutura subjacente, permitindo que os desenvolvedores se concentrem no código e na funcionalidade do aplicativo, sem se preocupar com a manutenção do hardware ou do sistema operacional.

- **SaaS (Software as a Service)**: Fornece aplicativos prontos para uso, acessíveis pela internet. O provedor é responsável pela manutenção, atualizações e segurança do software. Ao escolher um serviço SaaS, como um banco de dados, o Azure permite selecionar um servidor que será gerenciado pela Microsoft, garantindo sua operação e manutenção.

### Tabela de Modelo de Responsabilidade Compartilhada

A seguir, a tabela que ilustra o modelo de responsabilidade compartilhada entre o provedor de nuvem e o cliente, apresentada durante a aula:
![Modelo de Responsabilidade Compartilhada](https://github.com/Dani-dba/microsoft_azure_lab/commit/d9638dcc5e6649da68591114ea50a0348f495c43)


Durante a aula, foi demonstrado no portal do Azure como, ao selecionar configurações e a região do serviço, é possível verificar imediatamente o custo associado. Essa funcionalidade permite que os usuários tomem decisões informadas sobre a utilização de serviços em nuvem, otimizando custos e recursos.

**Este repositório será atualizado conforme avanço nos estudos e realizo novos laboratórios.**
