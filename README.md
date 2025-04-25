# 🌐 Resumo do Lab: Computação e Rede no Azure

Durante o desenvolvimento deste lab, explorei na prática como construir arquiteturas no Microsoft Azure, utilizando recursos essenciais voltados à computação, rede e banco de dados. O ambiente foi provisionado com foco em boas práticas de segurança, organização e otimização de custos.

---

## 🔧 Recursos Criados

- **Grupo de Recursos**: Estrutura lógica para organizar e gerenciar todos os recursos relacionados ao projeto.
  
- **Máquina Virtual (VM) com Windows**: Criação de uma VM baseada no sistema operacional Windows, com definição de tamanho, disco, e regras de acesso (como liberação da porta 3389 para RDP).
  
- **Rede Virtual (VNet)**: Configuração de uma rede privada para permitir a comunicação segura entre os recursos criados.

- **NSG (Network Security Group)**: Grupo de segurança de rede configurado para permitir apenas o tráfego necessário, protegendo a VM de acessos indevidos.

- **Azure SQL Database**: Banco de dados relacional na nuvem, gerenciado pela plataforma (PaaS), com autenticação via Azure AD, criptografia e acesso controlado pela VNet.

---

## ⚙️ Configuração e Dimensionamento de Máquinas Virtuais

Ao configurar as VMs no Azure, aprendi a importância de analisar e ajustar os seguintes aspectos:

- **Tamanho (SKU)**: Escolha do tipo de VM (quantidade de vCPUs, RAM, disco) conforme a carga de trabalho.
- **Tipo de Disco**: Optei por SSD padrão, equilibrando custo e desempenho.
- **Imagem de SO**: Utilização de imagens oficiais do Windows Server para estabilidade e suporte.
- **Região**: Os recursos foram criados na mesma região para garantir baixa latência e compatibilidade.
- **Desligamento Automático**: Recurso habilitado para evitar custos desnecessários fora do horário de uso.
- **Exclusão de Disco com a VM**: Habilitada a opção de excluir os discos junto com a VM para evitar armazenamento órfão gerando cobranças adicionais.
- **Diagnóstico e Monitoramento**: Logs de inicialização ativados para acompanhar o estado da VM e facilitar resolução de problemas.
- **Azure Bastion**: Utilizado para acessar a VM diretamente pelo navegador, sem expor IP público.

---

## ☁️ Conceitos Aprendidos

- **Provisionamento em Nuvem**: Organização e criação eficiente de recursos no Azure com foco em boas práticas.
- **Segurança e Acesso**: Configuração de acesso seguro à VM por meio de RDP via NSG e uso de Azure Bastion.
- **Rede Privada**: Criação de uma VNet para isolar e interligar recursos com segurança.
- **Banco de Dados como Serviço (DBaaS)**: Uso do Azure SQL Database, com autenticação moderna e sem necessidade de gerenciar infraestrutura.

---

## 🧠 Considerações Finais

Esse laboratório foi essencial para entender, de forma prática, como montar uma arquitetura funcional e segura no Azure. A experiência reforçou conceitos importantes de Infraestrutura como Serviço (IaaS) e Plataforma como Serviço (PaaS), além de destacar boas práticas como:

- Redução de custos com desligamento automático.
- Segurança de acesso com NSG e Bastion.
- Gerenciamento centralizado usando grupos de recursos.
- Planejamento adequado de regiões e redes.

---
