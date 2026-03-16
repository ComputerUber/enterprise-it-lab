# Enterprise LAN Design Project 2.0

This project represents an advanced enterprise network simulation developed as part of a network administration training program and expanded independently with additional infrastructure features.

The objective of this project was to design a resilient enterprise network capable of supporting multiple departments, internal services, redundancy mechanisms, and segmented network access.

The network was designed and simulated using Cisco Packet Tracer.

---

## Network Topology

![Network Topology](images/topology.png)

---

## Network Architecture Overview

The simulated infrastructure represents a medium-sized enterprise network with multiple departments and centralized services.

The network includes:

* Multiple Layer 3 switches for distribution and redundancy
* Dual ISP connectivity for internet failover
* Centralized gateway routing
* VLAN-based network segmentation
* Department-based resource access control
* Internal service infrastructure
* Backup and disaster recovery planning

---

## Internet Connectivity

The enterprise network uses dual ISP connectivity to improve availability.

The ISP routers operate in bridge mode and forward traffic to the central gateway device:

TP-Link ER8411

This allows centralized control of:

* routing
* firewall policies
* network segmentation
* WAN failover management

---

## VLAN Segmentation

Network segmentation was implemented using VLANs to isolate departments and improve security and performance.

Example VLAN structure:

* VLAN 1 – Helpdesk
* VLAN 2 – Administration
* VLAN 3 – Accounting and Coordination
* VLAN 5 – Sales
* VLAN 6 – Maintenance
* VLAN 7 – Internal Servers
* VLAN 8 – Web Services
* VLAN 10 – Guest WiFi Network
* VLAN 99 – IT Management

Each department operates in its own network segment.

---

## Inter-VLAN Routing

Routing between VLANs is handled through a hybrid architecture:

* Layer 3 switches manage internal network distribution
* The central gateway performs routing control and WAN connectivity

This hybrid design allows efficient traffic distribution within the network while maintaining centralized gateway control.

---

## Department Resource Isolation

Each department includes its own network printer.

Access control is enforced through VLAN segmentation, ensuring that:

* only devices within the same department VLAN can access their respective printer
* cross-department access is restricted

This approach improves both security and network organization.

---

## Infrastructure Components

The network includes several internal services:

* Web server
* File and storage services (NAS)
* Print server
* Backup server (standby)
* Internal communication systems

The backup server is intentionally kept offline and is designed to be activated only during:

* maintenance operations
* disaster recovery scenarios

---

## Network Resilience Features

The architecture includes several resilience mechanisms:

* Dual ISP internet connectivity
* Redundant switching paths
* VLAN segmentation
* Centralized gateway control
* Dedicated backup infrastructure

These features increase network reliability and fault tolerance.

---

## Technologies Used

* Cisco Packet Tracer
* VLAN segmentation
* Layer 3 switching
* Enterprise network topology design
* WAN redundancy concepts
* Network segmentation and resource isolation

---

## Author

Rui Filipe Silva

This project was developed as part of a networking training program and expanded independently to explore enterprise network architecture concepts.


# Laboratório de Administração de Rede Empresarial

Este projeto representa uma simulação avançada de uma rede empresarial desenvolvida no âmbito de um curso de administração de redes e posteriormente expandida de forma independente com funcionalidades adicionais de infraestrutura.

O objetivo deste projeto foi desenhar uma rede empresarial resiliente capaz de suportar vários departamentos, serviços internos, mecanismos de redundância e segmentação da rede.

A topologia foi criada utilizando o Cisco Packet Tracer.

---

## Visão Geral da Arquitetura

A infraestrutura simulada representa a rede de uma empresa de média dimensão com vários departamentos e serviços centralizados.

A rede inclui:

* Vários switches Layer 3 para distribuição e redundância
* Dupla ligação à Internet através de dois ISP
* Gateway central para controlo da rede
* Segmentação da rede através de VLANs
* Controlo de acesso a recursos por departamento
* Infraestrutura de serviços internos
* Planeamento de recuperação em caso de falha

---

## Conectividade à Internet

A rede utiliza duas ligações de ISP para garantir maior disponibilidade.

Os routers dos ISP encontram-se configurados em modo bridge e encaminham o tráfego para o gateway central:

TP-Link ER8411

Isto permite controlo centralizado de:

* routing
* políticas de firewall
* segmentação de rede
* failover de ligação WAN

---

## Segmentação de Rede (VLAN)

A rede foi segmentada através de VLANs para melhorar segurança, organização e desempenho.

Estrutura de VLANs:

* VLAN 1 – Helpdesk
* VLAN 2 – Administração
* VLAN 3 – Coordenação e Contabilidade
* VLAN 5 – Vendas
* VLAN 6 – Manutenção
* VLAN 7 – Servidores Internos
* VLAN 8 – Serviços Web
* VLAN 10 – Rede WiFi para convidados
* VLAN 99 – Gestão de TI

Cada departamento funciona na sua própria rede isolada.

---

## Routing entre VLANs

O routing entre VLANs utiliza uma arquitetura híbrida:

* switches Layer 3 gerem a distribuição interna da rede
* o gateway central gere o routing principal e a ligação WAN

Este modelo permite uma distribuição eficiente do tráfego na rede interna mantendo controlo centralizado.

---

## Isolamento de Recursos por Departamento

Cada departamento possui a sua própria impressora de rede.

A segmentação por VLAN garante que:

* apenas dispositivos do mesmo departamento conseguem aceder à sua impressora
* o acesso entre departamentos é restringido

---

## Infraestrutura de Serviços

A rede inclui vários serviços internos:

* servidor web
* armazenamento NAS
* servidor de impressão
* servidor de backup
* sistemas de comunicação interna

O servidor de backup encontra-se desligado por defeito e destina-se a ser utilizado apenas em cenários de:

* manutenção
* recuperação em caso de falha

---

## Mecanismos de Resiliência

A arquitetura inclui vários mecanismos de tolerância a falhas:

* dupla ligação à Internet
* caminhos redundantes entre switches
* segmentação VLAN
* gateway central de controlo
* infraestrutura de backup dedicada

---

## Tecnologias Utilizadas

* Cisco Packet Tracer
* VLAN
* Switching Layer 3
* Desenho de topologia de rede empresarial
* Conceitos de redundância WAN
* Segmentação e controlo de acesso

---

## Autor

Rui Filipe Silva
