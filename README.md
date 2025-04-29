# Criação de Máquina Virtual na Plataforma Microsoft Azure
## Introdução
---
Este repositório contém a documentação da minha experiência com a criação de uma máquina virtual na plataforma Microsoft Azure. Aqui, você encontrará um passo a passo detalhado de como criar uma máquina virtual no Azure, além de dicas e recursos adicionais.

## Requisitos
---
Conta no Microsoft Azure
Conhecimento básico de computação em nuvem

## Passo a Passo
---
1. Criar uma conta no Microsoft Azure
Acesse o site do Microsoft Azure e crie uma conta

Siga as instruções para criar uma conta gratuita

2. Criar uma máquina virtual
Acesse o portal do Azure e clique em "Máquinas Virtuais"

Clique em "Criar" e selecione a imagem do sistema operacional desejado

Configure as opções de hardware e rede

Clique em "Criar" para criar a máquina virtual

3. Conectar-se à máquina virtual
Acesse o portal do Azure e clique em "Máquinas Virtuais"

Selecione a máquina virtual criada e clique em "Conectar"

Use o protocolo RDP (Remote Desktop Protocol) para se conectar à máquina virtual

## Dicas e Recursos
---
Use o Azure CLI para criar e gerenciar máquinas virtuais 

Use o Azure Resource Manager para criar e gerenciar recursos no Azure

Acesse a documentação oficial do  [Aruze](https://learn.microsoft.com/pt-br/azure/?product=popular) para obter mais informações



## Conclusão
A criação de uma máquina virtual no Azure é um processo simples e rápido. Com este passo a passo, você pode criar sua própria máquina virtual no Azure e começar a explorar as funcionalidades da plataforma.

## Licença
Este repositório é licenciado sob a licença MIT. Você é livre para usar, modificar e distribuir o conteúdo deste repositório.


# 🧱 Componentes de Arquitetura do Azure

A arquitetura da Microsoft Azure é composta por diversos serviços e recursos que trabalham em conjunto para oferecer soluções escaláveis, seguras e de alta disponibilidade. Abaixo estão os principais componentes:
## 1. Recursos (Resources)

São os elementos individuais que você cria no Azure, como máquinas virtuais, bancos de dados, redes virtuais, entre outros.
## 2. Grupos de Recursos (Resource Groups)

Servem para organizar e gerenciar recursos relacionados. Um grupo de recursos pode conter vários recursos que compartilham o mesmo ciclo de vida.
## 3. Assinaturas (Subscriptions)

São usadas para organizar o acesso e o faturamento dos serviços. Cada assinatura possui limites e permissões definidas.
## 4. Azure Resource Manager (ARM)

É a camada de gerenciamento do Azure. Ele permite criar, atualizar e deletar recursos de forma organizada e segura, além de aplicar políticas e templates (ARM Templates).
## 5. Regiões e Zonas de Disponibilidade

    Regiões: locais geográficos onde os datacenters do Azure estão distribuídos (ex: Brazil South, East US).

    Zonas de Disponibilidade: áreas físicas independentes dentro de uma região para garantir alta disponibilidade.

## 6. Máquinas Virtuais (Virtual Machines - VMs)

Permitem a execução de sistemas operacionais e aplicações em servidores hospedados na nuvem.
## 7. Redes Virtuais (Virtual Networks - VNets)

Permitem a comunicação segura entre recursos do Azure e com redes locais.
## 8. Banco de Dados (Azure SQL, Cosmos DB, etc.)

Serviços gerenciados para armazenar dados estruturados e não estruturados, com alta escalabilidade e integração com outras soluções Azure.
## 9. Serviços de Identidade (Azure Active Directory)

Gerenciam usuários, autenticação e permissões de acesso aos recursos e aplicações.


