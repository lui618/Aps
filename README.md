
# 📘 Projeto de Sistema Computacional - "Termômetro da Felicidade"
<img width="192" height="89" alt="image" src="https://github.com/user-attachments/assets/9f00c432-def4-4de7-8b12-439b34ca8b9c" />

Curso: Superior de Tecnologia em Análise e Desenvolvimento de Sistemas

Disciplina: Análise e Projeto de Sistemas

Orientador: Prof. Me. Denys Alves da Silva

Alunos:  
         22451415 Luis Filipe Campelo Aragão Belinho luis.filipeb@sempreceub.com  
         22454566 Vinicius Mendes de Godoi vinicius.godoi@sempreceub.com  
         22450356 Jonatan Rodrigues Silva Corrêa jhonatan.correa@sempreceub.com  
         22452326 Cauã Gonçalves Xavier Mrad caua.xavier@sempreceub.com
         22450242 João Victor Alves Rodrigues joao.arodrigues@sempreceub.com  
         22404801 Maria Eduarda de Sousa Sales edurdasales@sempreceub.com 
         
      
---

## 📑 Sumário
1. [Documento de Visão do Sistema](#1-documento-de-visão-do-sistema)  
2. [Diagrama de Caso de Uso](#2-diagrama-de-caso-de-uso)  
3. [Especificação de Caso de Uso](#3-especificação-de-caso-de-uso)  
4. [Diagrama de Classe](#4-diagrama-de-classe)  
5. [Documento de Arquitetura do Sistema](#5-documento-de-arquitetura-do-sistema)  
6. [Protótipo do Sistema](#6-protótipo-do-sistema)  

---

## 1. Documento de Visão do Sistema

# 📖 Documento de Visão do Sistema - Termômetro da Felicidade

## 1. Introdução  
O sistema **Termômetro da Felicidade** tem como propósito apoiar organizações na **avaliação e acompanhamento do bem-estar e felicidade dos colaboradores**. Ele será uma ferramenta computacional de apoio à decisão, permitindo que gestores tenham indicadores claros e confiáveis sobre aspectos emocionais, sociais e profissionais dos funcionários, indo além de métricas tradicionais como produtividade e absenteísmo.  

---

## 2. Objetivos
Desenvolver um sistema de informação para avaliar o nível de felicidade no local de trabalho, facilitando decisões gerenciais sobre o bem-estar dos colaboradores.  

## 2.1 Benefícios Esperados

### Para a Gestão e Organização:
- Fornecer visibilidade em tempo real sobre o clima organizacional e variações de humor, permitindo **ações imediatas**.  
- Aumentar o **engajamento, a produtividade e a retenção de talentos**.  
- Subsidiar decisões gerenciais com **dados objetivos e contínuos**.  
- Reduzir custos associados ao **absenteísmo** e à **rotatividade de funcionários (turnover)**.  
- Aprimorar a cultura organizacional, fomentando um ambiente de **confiança e feedback contínuo**.  

### Para a Comunidade Acadêmica e Social:
- Contribuir com o avanço das áreas de **Sistemas de Informação** e **Engenharia de Software**.  
- Disponibilizar o sistema, a documentação e o código-fonte de forma **gratuita**, para que outras organizações possam adotá-lo e adaptá-lo.  

---

## 2.2 Público-Alvo
O público-alvo são **organizações**, com foco principal nas de **pequeno e médio porte**, que atualmente não dispõem de ferramentas adequadas para monitorar de forma sistemática e contínua o bem-estar e a felicidade de seus colaboradores.  

O sistema também se destina a **qualquer organização interessada** em adotar uma ferramenta gratuita para essa finalidade.  

--- 

## 3. Stakeholders  
- **Colaboradores**: respondem pesquisas e interagem com o sistema para medir bem-estar.  
- **Gestores e líderes**: utilizam relatórios e indicadores para tomada de decisão.  
- **Equipe de RH**: aplica ações de engajamento, treinamentos e acompanhamento.  
- **Administradores do sistema**: responsáveis pela configuração, manutenção e segurança da plataforma.  

## 4. Escopo

**O que está no escopo:**
- Coletar o grau de felicidade dos colaboradores de forma integrada ao momento do registro de ponto.  
- Apresentar aos gestores os resultados em tempo real por meio de um **dashboard**.  
- Disponibilizar o sistema para plataformas **Web e Mobile**.  
- Sugerir ações aos gestores com base nos dados coletados e na inteligência computacional.  
- Manter um histórico dos níveis de felicidade e das ações gerenciais realizadas.  

**O que não está no escopo:**
- O sistema não é uma ferramenta de registro de ponto, mas sim **integrado a ele**.  
- Não se trata de uma plataforma para terapia ou apoio psicológico direto, mas sim uma ferramenta de **monitoramento para gestão**.  
- O sistema não substituirá outros processos de Recursos Humanos, como **avaliação de desempenho ou controle de frequência**.  

## 5. Restrições  
- **Técnicas**: necessidade de integração segura com banco de dados; sistema deve ser responsivo (desktop e mobile).  
- **Orçamento**: foco em soluções acessíveis para pequenas e médias empresas, evitando altos custos de licenciamento.  
- **Prazos**: dependentes do cronograma de pesquisa e desenvolvimento.  
- **Requisitos obrigatórios**: confidencialidade dos dados, conformidade com a **LGPD**.  

## 6. Critérios de Sucesso  
- Pelo menos **70% dos colaboradores** participando das medições periódicas.  
- Adoção do sistema por pelo menos **X organizações piloto** em até 6 meses.  
- **Redução de absenteísmo ou turnover** nas organizações que utilizarem o sistema.  
- Feedback positivo de gestores quanto à usabilidade e utilidade dos relatórios.  
- Disponibilização pública do sistema e da documentação como contribuição científica e social.  

## 2. Diagrama de Caso de Uso

📌 **O que é:**  
Representação UML das **funcionalidades principais** e **atores envolvidos**.  

📌 **Como preencher:**  
- Identificar os atores (usuário, administrador, sistemas externos).  
- Identificar os casos de uso (funcionalidades).  
- Criar o diagrama em UML (PlantUML, Lucidchart, StarUML, Draw.io).  

📄 **Exemplo de atores e casos de uso:**  
- Atores: Usuário, Bibliotecário.  
- Casos de Uso: Realizar Login, Consultar Livro, Efetuar Empréstimo, Cadastrar Livro.  

📷 **Adicionar aqui o diagrama:**  
/docs/02-diagrama-caso-uso.png

---

## 3. Especificação de Caso de Uso

📌 **O que é:**  
Descrição detalhada do **fluxo principal e alternativo** de cada caso de uso.  

📌 **Modelo de Tabela:**  

| Item                  | Descrição |
|-----------------------|-----------|
| **Nome**              | Realizar Login |
| **Ator Principal**    | Usuário |
| **Pré-condições**     | Usuário já cadastrado no sistema |
| **Fluxo Principal**   | 1. Usuário insere login e senha <br> 2. Sistema valida credenciais <br> 3. Sistema libera acesso |
| **Fluxos Alternativos** | Senha incorreta → Sistema exibe mensagem de erro |
| **Pós-condições**     | Usuário autenticado no sistema |
| **Regras de negócio** | Senha deve ter no mínimo 8 caracteres |

📄 Criar uma tabela como esta **para cada caso de uso** identificado.

---

## 4. Diagrama de Classe

📌 **O que é:**  
Representação estática em UML das **classes, atributos, métodos e relacionamentos**.  

📌 **Como preencher:**  
- Listar classes principais (Ex.: Usuário, Livro, Empréstimo).  
- Definir atributos e métodos.  
- Relacionar com UML (herança, associação, composição, agregação).  

📷 **Adicionar aqui o diagrama:**  

/docs/04-diagrama-classes.png

---

## 5. Documento de Arquitetura do Sistema

📌 **O que é:**  
Definição da **estrutura técnica** do sistema.  

📌 **Como preencher:**  
- Visão geral da arquitetura (camadas ou microsserviços).  
- Tecnologias utilizadas (linguagem, frameworks, banco de dados).  
- Integrações externas (APIs, serviços).  
- Segurança (autenticação, criptografia).  
- Requisitos de desempenho e escalabilidade.  

📄 **Exemplo (preencher no projeto real):**  
Arquitetura em 3 camadas:

Apresentação (JavaFX ou ReactJS)

Negócio (Java - Spring Boot)

Persistência (MySQL)

Integrações: API de Pagamento
Segurança: Autenticação com JWT

---

## 6. Protótipo do Sistema

📌 **O que é:**  
Protótipo visual ou navegável que representa a interface do sistema.  

📌 **Como preencher:**  
- Criar esboços das telas principais (login, cadastro, dashboard).  
- Pode ser feito no **Figma, Balsamiq, Draw.io ou PowerPoint**.  
- Salvar em PDF ou imagem.  

📷 **Adicionar protótipo aqui:**  
/docs/06-prototipo.pdf

---

## ✅ Organização no GitHub
Estrutura de diretórios sugerida:

Arquivos de Markdown do GitHub para o aluno utilizar obrigatoriamente no seu projeto.

├── [1. Documento de Visão do Sistema](01-visao-sistema.md)

├── [2. Diagrama de Caso de Uso](02-diagrama-caso-uso.md)

├── [3. Especificação de Caso de Uso](03-especificacao-caso-uso.md)

├── [4. Diagrama de Classe](04-diagrama-classes.md)

├── [5. Documento de Arquitetura do Sistema](05-arquitetura-sistema.md)

├── [6. Protótipo do Sistema](06-prototipo.md)

---
