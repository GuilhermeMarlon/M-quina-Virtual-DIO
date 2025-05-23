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

📘 Conceitos Fundamentais do Azure

Este resumo aborda alguns conceitos essenciais sobre os serviços de infraestrutura e rede no Azure, com foco em contêineres, máquinas virtuais e conectividade entre redes.
# 🧩 1. Instâncias de Contêiner do Azure – Classificação

As Instâncias de Contêiner do Azure (Azure Container Instances - ACI) são classificadas como um serviço PaaS (Platform as a Service).
Esse modelo permite executar contêineres diretamente na nuvem sem necessidade de gerenciar máquinas virtuais ou orquestradores complexos. Você define a imagem do contêiner e as configurações, e o Azure cuida da infraestrutura subjacente.
# 🖥️ 2. Máquinas Virtuais vs. Contêineres
Característica	Máquinas Virtuais (VMs)	Contêineres
Sistema Operacional	Cada VM possui seu próprio SO	Compartilham o kernel do host
Isolamento do hardware	Sim	Não total
Tempo de inicialização	Mais lento	Mais rápido
Consumo de recursos	Mais pesado	Mais leve

# ✅ Verdadeiro: As VMs são isoladas do hardware do host, enquanto os contêineres não.

Isso significa que VMs simulam todo um computador, com hardware virtualizado, enquanto os contêineres compartilham o mesmo kernel do sistema operacional, embora isoladamente.
# 🔗 3. Comunicação entre Redes Virtuais (VNets)

Para que duas Redes Virtuais (VNets) distintas possam se comunicar, é necessário configurar o Emparelhamento de Redes (VNet Peering).

    O emparelhamento permite a troca de tráfego entre redes virtuais de forma segura e eficiente, como se estivessem na mesma rede.

    Ele pode ser feito entre redes na mesma região (regional) ou entre regiões diferentes (global).

# 🌐 4. Conexão Privada com a Azure – ExpressRoute

O ExpressRoute é um serviço que permite estender sua rede local até o Azure por meio de uma conexão privada (não passando pela internet pública).

    É facilitado por um provedor de conectividade.

    Garante maior segurança, confiabilidade, latência reduzida e largura de banda mais alta.

    Ideal para empresas que precisam de alto desempenho em integração entre nuvem e data center local.


# 🔐 Identidade, Acesso e Segurança no Azure

A segurança na nuvem é baseada em princípios sólidos que garantem a proteção de dados, sistemas e identidades contra acessos não autorizados. A seguir, veja uma explicação detalhada dos principais conceitos:
# 🛡️ Defesa em Profundidade

Defesa em profundidade é uma estratégia de segurança que utiliza múltiplas camadas de proteção, dificultando o progresso de um ataque ao sistema. A ideia central é que, mesmo que uma camada seja violada, outras estarão presentes para impedir o acesso não autorizado.

## Camadas comuns da defesa em profundidade:

    Física: segurança do datacenter.

    Perímetro: firewalls, IDS/IPS, roteadores seguros.

    Rede: segmentação de rede, NSGs.

    Computação: VMs seguras, patches atualizados.

    Aplicação: validação de entrada, WAFs.

    Acesso e identidade: autenticação, autorização.

    Dados: criptografia, classificação, controle de acesso.

# 👁️‍🗨️ Autenticação Multifator (MFA)

 MFA (Multi-Factor Authentication) é uma camada extra de segurança que exige dois ou mais fatores para autenticar um usuário:

    Algo que você sabe: senha ou PIN.

    Algo que você possui: celular, token ou smartcard.

    Algo que você é: biometria (impressão digital, reconhecimento facial, etc.).

Essa abordagem reduz significativamente o risco de acessos indevidos, mesmo quando senhas são comprometidas.
# 🌐 Camada de Perímetro (Perimeter Layer)

A camada de perímetro na defesa em profundidade tem o papel de bloquear ou detectar ataques vindos da rede externa antes que eles atinjam a infraestrutura interna.

## Ferramentas e práticas incluem:

    Firewalls.

    IDS/IPS (Sistemas de detecção e prevenção de intrusão).

    VPNs.

    DDoS Protection.

    Edge routers seguros.

Ela representa a primeira linha de defesa contra ameaças externas.
# 🧾 Microsoft Entra ID (antigo Azure AD)

Microsoft Entra ID é o serviço de gerenciamento de identidades e acesso baseado em nuvem do Azure. Ele permite autenticar e autorizar usuários e dispositivos em ambientes híbridos (nuvem e local).

## Principais recursos:

    Autenticação e SSO.

    Autenticação multifator (MFA).

    Acesso condicional.

    Integração com milhares de aplicativos SaaS.

    Gerenciamento de grupos e funções.

O Entra ID ajuda a aplicar políticas de segurança, controle de acesso e governança de identidade de forma centralizada.
# 🧭 Conceitos-Chave: Identidade, Acesso e Segurança

    Identidade: quem você é (usuário, dispositivo ou sistema). Ex: conta de usuário.

    Acesso: o que você pode fazer ou ver. Ex: permissões em recursos.

    Segurança: mecanismos que protegem o ambiente contra acessos não autorizados, vazamentos ou ataques. Ex: criptografia, autenticação, políticas de acesso.

Esses três pilares são a base de qualquer arquitetura segura na nuvem.


