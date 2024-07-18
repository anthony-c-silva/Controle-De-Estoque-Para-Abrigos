# Documento de Requisitos

## Controle de Estoque para Abrigos

Anthony C. Silva, Luiz Felipe Cavalheiro

05/06/2024

## 1. Introdução

### 1.1 Propósito
O propósito deste documento é detalhar os requisitos funcionais e não funcionais do sistema de Controle de Estoque para Abrigos. Este documento servirá como guia para o desenvolvimento e validação do sistema.

### 1.2 Escopo
O sistema será um aplicativo web destinado a gerenciar o estoque de abrigos, incluindo o registro de doações e a estimativa de necessidades futuras. O projeto incluirá um front-end em React, um back-end em Express.js e um banco de dados PostgreSQL.

### 1.3 Definições, Acrônimos e Abreviações
- **CRUD**: Create, Read, Update, Delete
- **ORM**: Object-Relational Mapping
- **RF**: Requisito Funcional
- **RNF**: Requisito Não Funcional

## 2. Requisitos Funcionais

### 2.1 Gerenciamento de Itens
- **RF01**: O sistema deve permitir o cadastro de novos itens no estoque.
- **RF02**: O sistema deve permitir a atualização de informações dos itens no estoque.
- **RF03**: O sistema deve permitir a remoção de itens do estoque.
- **RF04**: O sistema deve exibir uma lista de todos os itens no estoque, incluindo nome, quantidade, categoria e abrigo associado.

### 2.2 Gerenciamento de Usuários
- **RF05**: O sistema deve permitir o cadastro de novos usuários.
- **RF06**: O sistema deve permitir a atualização de informações dos usuários.
- **RF07**: O sistema deve permitir a remoção de usuários.
- **RF08**: O sistema deve implementar autenticação para garantir que apenas usuários autorizados possam acessar funcionalidades específicas.

### 2.3 Gerenciamento de Abrigos
- **RF09**: O sistema deve permitir o cadastro de novos abrigos.
- **RF10**: O sistema deve permitir a atualização de informações dos abrigos.
- **RF11**: O sistema deve permitir a remoção de abrigos.
- **RF12**: O sistema deve permitir a associação de itens e usuários a um abrigo específico.

### 2.4 Gerenciamento de Doações
- **RF13**: O sistema deve permitir o registro de novas doações, especificando item, quantidade, data e doador.
- **RF14**: O sistema deve permitir a atualização de informações das doações.
- **RF15**: O sistema deve permitir a remoção de doações.
- **RF16**: O sistema deve exibir um histórico de todas as doações recebidas.

### 2.5 Estimativa de Necessidades
- **RF17**: O sistema deve permitir a simulação de cenários para estimar as necessidades futuras de itens.
- **RF18**: O sistema deve gerar relatórios de estimativas baseados em dados históricos e previsões.

## 3. Requisitos Não Funcionais

### 3.1 Usabilidade
- **RNF01**: O sistema deve possuir uma interface intuitiva e de fácil uso.
- **RNF02**: O sistema deve ser responsivo, adaptando-se a diferentes tamanhos de tela e dispositivos.

### 3.2 Confiabilidade
- **RNF03**: O sistema deve ser robusto, garantindo a integridade dos dados durante operações CRUD.
- **RNF04**: O sistema deve implementar backups regulares do banco de dados.

### 3.3 Performance
- **RNF05**: O sistema deve responder a requisições em no máximo 2 segundos.
- **RNF06**: O sistema deve suportar pelo menos 100 usuários simultâneos sem degradação perceptível de desempenho.

### 3.4 Segurança
- **RNF07**: O sistema deve garantir a segurança dos dados, implementando autenticação e autorização adequadas.
- **RNF08**: O sistema deve proteger os dados de usuários e doações usando criptografia.

### 3.5 Manutenibilidade
- **RNF09**: O sistema deve ser desenvolvido usando padrões de código limpo e bem documentado.
- **RNF10**: O sistema deve permitir fácil modificação e extensão para novas funcionalidades.

### 3.6 Portabilidade
- **RNF11**: O sistema deve ser compatível com os principais navegadores web (Chrome, Firefox, Safari, Edge).
- **RNF12**: O sistema deve ser hospedado em plataformas modernas de cloud computing (e.g., Vercel, Heroku).

## 4. Casos de Uso

### 4.1 Caso de Uso 1: Gerenciar Itens
**Descrição**: Permite aos usuários cadastrar, atualizar, visualizar e remover itens do estoque.  
**Ator(es)**: Gestores de Estoques

### 4.2 Caso de Uso 2: Gerenciar Usuários
**Descrição**: Permite aos administradores cadastrar, atualizar, visualizar e remover usuários do sistema.  
**Ator(es)**: Administradores

### 4.3 Caso de Uso 3: Gerenciar Abrigos
**Descrição**: Permite aos usuários cadastrar, atualizar, visualizar e remover abrigos, bem como associar itens e usuários a abrigos específicos.  
**Ator(es)**: Gestores de Estoques, Administradores

### 4.4 Caso de Uso 4: Gerenciar Doações
**Descrição**: Permite aos usuários registrar, atualizar, visualizar e remover doações.  
**Ator(es)**: Gestores de Estoques, Voluntários

### 4.5 Caso de Uso 5: Estimar Necessidades
**Descrição**: Permite aos usuários simular cenários para estimar necessidades futuras de itens.  
**Ator(es)**: Gestores de Estoques

## 5. Interfaces do Usuário

### 5.1 Interface de Login
**Descrição**: Tela para autenticação dos usuários.

### 5.2 Interface de Cadastro de Itens
**Descrição**: Tela para cadastro e gerenciamento de itens no estoque.

### 5.3 Interface de Gerenciamento de Usuários
**Descrição**: Tela para cadastro e gerenciamento de usuários.

### 5.4 Interface de Gerenciamento de Abrigos
**Descrição**: Tela para cadastro e gerenciamento de abrigos.

### 5.5 Interface de Registro de Doações
**Descrição**: Tela para registro e gerenciamento de doações.

### 5.6 Interface de Estimativa de Necessidades
**Descrição**: Tela para simulação de cenários e estimativa de necessidades futuras de itens.

## 6. Restrições

- **R01**: O sistema deve estar operacional 99.9% do tempo.
- **R02**: O desenvolvimento deve ser concluído em 6 meses.
- **R03**: O sistema deve ser desenvolvido usando as tecnologias especificadas (React, Express.js, PostgreSQL).

## 7. Aceitação e Validação

### 7.1 Critérios de Aceitação
- **CA01**: Todas as funcionalidades devem estar implementadas conforme os requisitos especificados.
- **CA02**: O sistema deve passar por testes de usabilidade e segurança.
- **CA03**: O desempenho do sistema deve ser validado em cenários de alta carga.

### 7.2 Plano de Testes
- **PT01**: Testes unitários para todas as funções críticas.
- **PT02**: Testes de integração para assegurar a interação correta entre os componentes do sistema.
- **PT03**: Testes de aceitação com usuários finais.
