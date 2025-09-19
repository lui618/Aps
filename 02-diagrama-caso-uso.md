# 🎭 Diagrama de Caso de Uso

## 1. Introdução
O Diagrama de Casos de Uso é uma representação visual das funcionalidades do sistema e das interações entre atores externos (usuários, sistemas) e o próprio sistema. No contexto do Termômetro da Felicidade, o diagrama ajuda a:

esclarecer quem usa o sistema (colaboradores, gestores, administradores e sistemas externos) e por quê;

priorizar requisitos funcionais (coleta de felicidade, dashboards, recomendações, integração com ponto);

fornecer uma visão simples para validação com stakeholders antes da modelagem mais detalhada (classes, sequências e componentes).
Este diagrama será a base para os demais artefatos UML e garante rastreabilidade entre requisitos e design. (Base: Documento de Visão / Projeto PIC). 

## 2. Atores Identificados
Colaborador — fornece o nível de felicidade (registro rápido no momento do ponto), participa da gamificação, visualiza seu histórico pessoal.

Gestor — visualiza dashboards da equipe, recebe recomendações de ações, aplica intervenções e acompanha efeitos ao longo do tempo.

Diretor — visão executiva (KPIs organizacionais), aprova políticas e ações estratégicas.

Administrador do Sistema — gerencia usuários, permissões, configura integrações e parâmetros do sistema (limiares, regras de gamificação).

Analista de Dados / RH — gera relatórios avançados, exporta dados, realiza análises e treina/ajusta modelos de recomendação.

Sistema de Registro de Ponto (externo) — sistema de ponto eletrônico que dispara/integra a coleta do nível de felicidade no momento do registro.

Serviço de Notificação (externo) — serviço de envio de e-mail/SMS/push para alertas e campanhas.

Serviço de Autenticação/SSO (externo) — provê autenticação centralizada (se houver SSO). 

## 3. Casos de Uso
A seguir são apresentados os principais casos de uso do sistema Termômetro da Felicidade, descrevendo de forma resumida os atores envolvidos, o objetivo de cada funcionalidade, suas pré-condições e o fluxo principal de execução.

3.1 Realizar Login — Todos os Usuários

Descrição: Permite que qualquer usuário acesse o sistema por meio de autenticação.

Pré-condição: O usuário deve estar previamente cadastrado.

Fluxo Principal: O usuário insere suas credenciais → o sistema valida os dados → a sessão é iniciada.

3.2 Registrar Grau de Felicidade — Colaborador

Descrição: O colaborador registra seu nível de felicidade (ex.: escala de 1 a 5), podendo incluir um comentário.

Pré-condição: O colaborador deve estar autenticado.

Fluxo Principal: O sistema apresenta formulário → o colaborador insere nível/comentário → os dados são salvos → pontos de gamificação são atribuídos.

3.3 Registrar Grau via Integração com Ponto — Sistema de Ponto (externo)

Descrição: Ao registrar o ponto, o sistema solicita automaticamente o grau de felicidade do colaborador.

Pré-condição: O colaborador deve estar autenticado no momento do registro de ponto.

Fluxo Principal: O Sistema de Ponto envia evento → o sistema exibe formulário de felicidade → o colaborador insere o dado → registro armazenado.

3.4 Visualizar Histórico Pessoal — Colaborador

Descrição: Permite ao colaborador acompanhar sua evolução de felicidade ao longo do tempo.

Pré-condição: O colaborador deve estar autenticado.

Fluxo Principal: O colaborador acessa o menu de histórico → o sistema recupera os registros → apresenta lista e gráficos individuais.

3.5 Participar de Gamificação — Colaborador

Descrição: O colaborador acumula pontos por participação e pode visualizar rankings ou recompensas.

Pré-condição: Deve existir pelo menos um registro de felicidade válido.

Fluxo Principal: O sistema soma pontos → atualiza posição do usuário → exibe ranking e conquistas.

3.6 Visualizar Dashboard da Equipe — Gestor

Descrição: Permite ao gestor analisar os indicadores de felicidade de sua equipe.

Pré-condição: O usuário deve estar autenticado como gestor.

Fluxo Principal: O gestor solicita o dashboard → o sistema agrega os dados da equipe → apresenta gráficos, médias e alertas.

3.7 Receber Sugestões de Ações — Gestor

Descrição: O sistema recomenda ações baseadas na análise dos níveis de felicidade da equipe.

Pré-condição: Deve haver registros recentes de felicidade coletados.

Fluxo Principal: O motor de análise processa os dados → gera recomendações → o gestor visualiza → pode aceitar ou rejeitar a sugestão.

3.8 Visualizar Indicadores Organizacionais — Diretor

Descrição: Fornece ao diretor uma visão consolidada dos indicadores gerais da organização.

Pré-condição: O usuário deve estar autenticado como diretor.

Fluxo Principal: O diretor acessa o painel → o sistema recupera dados de todas as equipes → apresenta comparativos, KPIs e tendências históricas.

3.9 Gerenciar Usuários e Permissões — Administrador

Descrição: Permite cadastrar, editar ou remover usuários, bem como atribuir papéis de acesso (colaborador, gestor, diretor).

Pré-condição: O usuário deve estar autenticado como administrador.

Fluxo Principal: O administrador acessa o menu de gestão → seleciona operação desejada → o sistema aplica as alterações e salva no banco de dados.

3.10 Configurar Integração com Ponto — Administrador

Descrição: Permite definir os parâmetros técnicos de integração entre o sistema e o registro de ponto eletrônico.

Pré-condição: O usuário deve estar autenticado como administrador.

Fluxo Principal: O administrador acessa a tela de integração → preenche endpoints e tokens → o sistema valida → configuração salva.

## 4. Diagrama UML
![diagramauml](image-2.png)
