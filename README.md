
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



# 1. Documento de Visão do Sistema - Termômetro da Felicidade

## 1.1 Introdução  
O sistema **Termômetro da Felicidade** tem como propósito apoiar organizações na **avaliação e acompanhamento do bem-estar e felicidade dos colaboradores**. Ele será uma ferramenta computacional de apoio à decisão, permitindo que gestores tenham indicadores claros e confiáveis sobre aspectos emocionais, sociais e profissionais dos funcionários, indo além de métricas tradicionais como produtividade e absenteísmo.  

---

## 1.2 Objetivos
Desenvolver um sistema de informação para avaliar o nível de felicidade no local de trabalho, facilitando decisões gerenciais sobre o bem-estar dos colaboradores.  

## 1.3 Benefícios Esperados

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

## 1.4 Público-Alvo
O público-alvo são **organizações**, com foco principal nas de **pequeno e médio porte**, que atualmente não dispõem de ferramentas adequadas para monitorar de forma sistemática e contínua o bem-estar e a felicidade de seus colaboradores.  

O sistema também se destina a **qualquer organização interessada** em adotar uma ferramenta gratuita para essa finalidade.  

--- 

## 1.5 Stakeholders  
- **Colaboradores**: respondem pesquisas e interagem com o sistema para medir bem-estar.  
- **Gestores e líderes**: utilizam relatórios e indicadores para tomada de decisão.  
- **Equipe de RH**: aplica ações de engajamento, treinamentos e acompanhamento.  
- **Administradores do sistema**: responsáveis pela configuração, manutenção e segurança da plataforma.  

## 1.6 Escopo

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

## 1.7 Restrições  
- **Técnicas**: necessidade de integração segura com banco de dados; sistema deve ser responsivo (desktop e mobile).  
- **Orçamento**: foco em soluções acessíveis para pequenas e médias empresas, evitando altos custos de licenciamento.  
- **Prazos**: dependentes do cronograma de pesquisa e desenvolvimento.  
- **Requisitos obrigatórios**: confidencialidade dos dados, conformidade com a **LGPD**.  

## 1.8 Critérios de Sucesso  
- Pelo menos **70% dos colaboradores** participando das medições periódicas.  
- Adoção do sistema por pelo menos **X organizações piloto** em até 6 meses.  
- **Redução de absenteísmo ou turnover** nas organizações que utilizarem o sistema.  
- Feedback positivo de gestores quanto à usabilidade e utilidade dos relatórios.  
- Disponibilização pública do sistema e da documentação como contribuição científica e social.  

## 2. Diagrama de Caso de Uso

## 2.1 Introdução

O Diagrama de Casos de Uso representa as principais funcionalidades do sistema Termômetro da Felicidade e as interações entre os diferentes atores (usuários e sistemas externos).
Essa visão facilita a compreensão das responsabilidades de cada papel e apoia a priorização dos requisitos funcionais do projeto.

O modelo destaca as operações de login, coleta e acompanhamento de felicidade, gamificação, sugestões, dashboards e integrações administrativas.
Ele também serve como base para os demais artefatos UML, garantindo rastreabilidade entre requisitos e design.

## 2.2 Atores Identificados

Colaborador — Registra e acompanha seu grau de felicidade, participa de gamificação e pode enviar sugestões.<br>
Gestor — Acompanha os indicadores de felicidade da equipe e recebe sugestões enviadas pelos colaboradores.<br>
Diretor — Visualiza o dashboard geral da equipe para análise organizacional.<br>
Administrador — Gerencia usuários, permissões e configurações de integração com o sistema de ponto.<br>
Sistema de Ponto (externo) — Sistema de registro de ponto da organização que poderá enviar uma mensagem como link para o colaborador motivando o colaborador a informar seu grau de felicidade no momento, possibilitando o vínculo automático com a coleta de felicidade.<br>

## 2.3 Casos de Uso Identificados
2.3.1 Realizar Login — Todos os Usuários
2.3.2 Cadastrar, Editar e Excluir Conta — Administrador / Colaborador
2.3.3 Responder Questionário de Felicidade — Colaborador
2.3.4 Registrar Grau de Felicidade Anônimo — Colaborador
2.3.5 Participar de Gamificação — Colaborador
2.3.6 Enviar Sugestão — Colaborador
2.3.7 Visualizar Histórico Pessoal — Colaborador
2.3.8 Visualizar Dashboard da Equipe — Gestor / Diretor
2.3.9 Receber Sugestões — Gestor
2.3.10 Gerenciar Usuários e Permissões — Administrador
2.3.11 Configurar Integração com Ponto — Administrador
2.3.12 Enviar Registro de Ponto — Sistema de Ponto (Externo) / Colaborador

## 2.4 Diagrama UML
![alt text](image-1.png)

---

## 3. Especificação de Caso de Uso

# 📝 Especificação de Casos de Uso – Termômetro da Felicidade

## 3.1 Realizar Login
| Item                 | Descrição |
|----------------------|-----------|
| **Nome**             | Realizar Login |
| **Ator Principal**   | Usuário (Colaborador, Gestor, Diretor, Administrador) |
| **Pré-condições**    | Usuário já cadastrado no sistema |
| **Fluxo Principal**  | 1. Usuário insere login e senha <br> 2. Sistema valida credenciais <br> 3. Sistema libera acesso |
| **Fluxos Alternativos** | Senha incorreta → Sistema exibe mensagem de erro |
| **Pós-condições**    | Usuário autenticado no sistema |
| **Regras de negócio**| Senha deve ter no mínimo 8 caracteres |

---

## 3.2.1 Cadastrar Conta
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Cadastrar Conta |
| **Ator Principal** | Colaborador / Administrador |
| **Pré-condições**  | Usuário autenticado com permissões adequadas |
| **Fluxo Principal**| 1. Usuário acessa tela de cadastro <br> 2. Preenche dados obrigatórios <br> 3. Sistema valida e cria a conta |
| **Fluxos Alternativos** | Dados inválidos → Sistema solicita correção |
| **Pós-condições**  | Conta criada com sucesso |

---

## 3.2.2 Editar Conta
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Editar Conta |
| **Ator Principal** | Colaborador / Administrador |
| **Pré-condições**  | Usuário autenticado |
| **Fluxo Principal**| 1. Usuário acessa sua conta <br> 2. Altera dados desejados <br> 3. Sistema valida e confirma alterações |
| **Fluxos Alternativos** | Dados inválidos → Sistema solicita correção |
| **Pós-condições**  | Dados atualizados com sucesso |

---

## 3.2.3 Excluir Conta
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Excluir Conta |
| **Ator Principal** | Administrador |
| **Pré-condições**  | Administrador autenticado |
| **Fluxo Principal**| 1. Administrador seleciona conta <br> 2. Sistema exibe confirmação <br> 3. Conta é removida do sistema |
| **Fluxos Alternativos** | Se usuário tentar excluir sua própria conta → Sistema bloqueia ação |
| **Pós-condições**  | Conta removida do sistema |

---

## 3.3 Responder Questionário de Felicidade
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Responder Questionário de Felicidade |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Colaborador autenticado no sistema |
| **Fluxo Principal**| 1. Sistema exibe questionário <br> 2. Colaborador responde <br> 3. Sistema registra no histórico |
| **Fluxos Alternativos** | Conexão perdida → Sistema salva parcialmente e retoma |
| **Pós-condições**  | Registro salvo no histórico pessoal |
| **Relações**       | `<<include>> Registrar Grau de Felicidade Anônimo` <br> `<<extend>> Participar de Gamificação / Enviar Sugestão` |

---

## 3.4 Registrar Grau de Felicidade Anônimo
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Registrar Grau de Felicidade Anônimo |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Acesso ao questionário ativo |
| **Fluxo Principal**| 1. Colaborador responde questionário <br> 2. Sistema salva resposta sem vínculo com identidade |
| **Pós-condições**  | Registro anônimo armazenado |
| **Relações**       | `<<include>> do Questionário de Felicidade` |

---

## 3.5 Participar de Gamificação
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Participar de Gamificação |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Respostas válidas no questionário |
| **Fluxo Principal**| 1. Colaborador participa respondendo <br> 2. Sistema gera pontos e atualiza ranking |
| **Pós-condições**  | Colaborador pontua na gamificação |
| **Relações**       | `<<extend>> do Questionário de Felicidade` |

---

## 3.6 Enviar Sugestão
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Enviar Sugestão |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Colaborador autenticado |
| **Fluxo Principal**| 1. Colaborador escreve sugestão <br> 2. Sistema registra e envia ao Gestor |
| **Pós-condições**  | Sugestão disponível para gestores |
| **Relações**       | `<<extend>> do Questionário de Felicidade` |

---

## 3.7 Visualizar Histórico Pessoal
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Visualizar Histórico Pessoal |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Colaborador autenticado |
| **Fluxo Principal**| 1. Colaborador acessa histórico <br> 2. Sistema exibe registros passados |
| **Pós-condições**  | Histórico exibido para análise individual |

---

## 3.8 Visualizar Dashboard da Equipe
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Visualizar Dashboard da Equipe |
| **Ator Principal** | Gestor / Diretor |
| **Pré-condições**  | Usuário autenticado |
| **Fluxo Principal**| 1. Usuário acessa dashboard <br> 2. Sistema processa e apresenta gráficos |
| **Pós-condições**  | Indicadores exibidos para tomada de decisão |

---

## 3.9 Receber Sugestões
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Receber Sugestões |
| **Ator Principal** | Gestor |
| **Pré-condições**  | Sugestões enviadas por colaboradores |
| **Fluxo Principal**| 1. Sistema lista sugestões <br> 2. Gestor visualiza e avalia |
| **Pós-condições**  | Sugestões ficam disponíveis para análise |

---

## 3.10 Gerenciar Usuários e Permissões
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Gerenciar Usuários e Permissões |
| **Ator Principal** | Administrador |
| **Pré-condições**  | Administrador autenticado |
| **Fluxo Principal**| 1. Administrador acessa painel de usuários <br> 2. Adiciona, altera ou remove permissões |
| **Pós-condições**  | Usuários e papéis atualizados |

---

## 3.11 Configurar Integração com Ponto
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Configurar Integração com Ponto |
| **Ator Principal** | Administrador |
| **Pré-condições**  | Administrador autenticado |
| **Fluxo Principal**| 1. Admin insere parâmetros técnicos <br> 2. Sistema valida <br> 3. Configuração salva |
| **Pós-condições**  | Integração habilitada |

---

## 3.12 Enviar Registro de Ponto
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Enviar Registro de Ponto |
| **Ator Principal** | Sistema de Ponto (Externo) |
| **Pré-condições**  | Sistema de ponto ativo |
| **Fluxo Principal**| 1. Colaborador registra entrada <br> 2. Sistema de ponto envia dados ao Termômetro <br> 3. Sistema solicita grau de felicidade |
| **Pós-condições**  | Registro de ponto vinculado ao questionário de felicidade |


---
