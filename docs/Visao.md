# Documento de Visão

## Controle de Estoque para Abrigos

Anthony C. Silva, Luiz Felipe Cavalheiro

05/06/2024

## 1. Introdução

### 1.1 Propósito
O propósito deste documento é fornecer uma visão clara e concisa do projeto de Controle de Estoque para Abrigos. Ele descreve os objetivos, o escopo, as funcionalidades principais, os usuários-alvo e outras informações relevantes para garantir que todas as partes interessadas tenham uma compreensão comum do projeto.

### 1.2 Escopo
O projeto visa desenvolver um aplicativo web simplificado para o controle de estoque de abrigos, com funcionalidades de gerenciamento de doações e estimativas de necessidades em diferentes cenários. A aplicação será composta por um front-end desenvolvido em React, um back-end em Express.js, e um banco de dados PostgreSQL.

## 2. Descrição Geral

### 2.1 Contexto
Nos abrigos, a gestão eficiente de doações e itens de estoque é crucial para garantir que as necessidades dos residentes sejam atendidas de forma oportuna. Este sistema busca simplificar o gerenciamento de estoques, permitindo uma visão clara das doações recebidas e das necessidades futuras, facilitando a tarefa dos gestores de estoque.

### 2.2 Objetivos
- Simplificar o gerenciamento de doações e estoques em abrigos.
- Prover uma interface intuitiva para a entrada e visualização de dados.
- Estimar necessidades futuras de itens com base em cenários simulados.
- Facilitar a tomada de decisões para os gestores de abrigos.

## 3. Funcionalidades Principais

### 3.1 Gerenciamento de Itens
- **Adicionar/Atualizar/Remover Itens**: Permitir que os usuários cadastrem novos itens, atualizem informações existentes ou removam itens que não são mais necessários.
- **Visualizar Estoque**: Mostrar uma lista de todos os itens disponíveis no estoque, incluindo detalhes como nome, quantidade, categoria e abrigo associado.

### 3.2 Gerenciamento de Usuários
- **Autenticação e Autorização**: Controle de acesso para garantir que apenas usuários autorizados possam acessar determinadas funcionalidades.
- **Gerenciamento de Perfis**: Adicionar, atualizar ou remover usuários do sistema.

### 3.3 Gerenciamento de Abrigos
- **Adicionar/Atualizar/Remover Abrigos**: Gerenciar informações sobre diferentes abrigos, incluindo nome e localização.
- **Associação de Itens e Usuários a Abrigos**: Facilitar a associação de itens e usuários específicos a um abrigo.

### 3.4 Gerenciamento de Doações
- **Registro de Doações**: Permitir o registro de doações recebidas, especificando item, quantidade, data e doador.
- **Histórico de Doações**: Manter um histórico de todas as doações recebidas e associar doações a itens específicos.

### 3.5 Estimativa de Necessidades
- **Simulação de Cenários**: Permitir que os usuários simulem diferentes cenários para estimar as necessidades futuras de itens com base em dados históricos e previsões.

## 4. Público-Alvo

### 4.1 Gestores de Estoques/Abrigos
Os principais usuários do sistema serão os gestores responsáveis pelo controle de estoques nos abrigos. Eles utilizarão a aplicação para gerenciar doações, visualizar e atualizar o inventário, e estimar necessidades futuras.

### 4.2 Voluntários
Voluntários que auxiliam na gestão do estoque também poderão usar o sistema para registrar doações e manter o inventário atualizado.

## 5. Requisitos do Sistema

### 5.1 Requisitos Funcionais
- **RF01**: O sistema deve permitir o cadastro, atualização e remoção de itens.
- **RF02**: O sistema deve permitir o cadastro, atualização e remoção de usuários.
- **RF03**: O sistema deve permitir o cadastro, atualização e remoção de abrigos.
- **RF04**: O sistema deve permitir o registro e visualização de doações.
- **RF05**: O sistema deve fornecer ferramentas para a estimativa de necessidades futuras de itens.

### 5.2 Requisitos Não Funcionais
- **RNF01**: O sistema deve ser acessível via web.
- **RNF02**: O sistema deve garantir a segurança dos dados, com autenticação e autorização adequadas.
- **RNF03**: O sistema deve ser responsivo e funcionar em dispositivos móveis e desktops.
- **RNF04**: O sistema deve ter alta disponibilidade e desempenho adequado para uso diário.
- **RNF05**: O sistema deve ser escalável para suportar múltiplos abrigos e grandes quantidades de dados.

## 6. Tecnologias Utilizadas
- **Front-end**: React
- **Back-end**: Node.js com Type Script
- **Banco de Dados**: PostgreSQL
- **ORM**: Prisma
- **Hospedagem do Back-end**: Render
- **Hospedagem do Banco de Dados**: Render

## 7. Conclusão
Este documento de visão fornece um panorama completo do projeto de Controle de Estoque para Abrigos, estabelecendo uma base sólida para o desenvolvimento e implementação do sistema. O próximo passo é iniciar o desenvolvimento conforme as especificações aqui descritas, garantindo que todos os requisitos sejam atendidos e que o sistema seja entregue com sucesso aos usuários finais.
