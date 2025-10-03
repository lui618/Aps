# 🎭 Diagrama de Caso de Uso

## 1. Introdução

O Diagrama de Casos de Uso representa as principais funcionalidades do sistema Termômetro da Felicidade e as interações entre os diferentes atores (usuários e sistemas externos).
Essa visão facilita a compreensão das responsabilidades de cada papel e apoia a priorização dos requisitos funcionais do projeto.

O modelo destaca as operações de login, coleta e acompanhamento de felicidade, gamificação, sugestões, dashboards e integrações administrativas.
Ele também serve como base para os demais artefatos UML, garantindo rastreabilidade entre requisitos e design.

## 2. Atores Identificados

Colaborador — Registra e acompanha seu grau de felicidade, participa de gamificação e pode enviar sugestões.
Gestor — Acompanha os indicadores de felicidade da equipe e recebe sugestões enviadas pelos colaboradores.
Diretor — Visualiza o dashboard geral da equipe para análise organizacional.
Administrador — Gerencia usuários, permissões e configurações de integração com o sistema de ponto.
Sistema de Ponto (externo) — Envia registros de ponto ao sistema principal, possibilitando o vínculo automático com a coleta de felicidade.

## 3. Casos de Uso
3.1 Realizar Login — Todos os Usuários

Descrição: Permite que qualquer usuário autenticado acesse o sistema.
Pré-condição: O usuário deve possuir uma conta cadastrada.
Fluxo Principal: O usuário informa credenciais → o sistema valida → o acesso é concedido.

3.2 Cadastrar, Editar e Excluir Conta — Administrador / Colaborador

Descrição: Permite o gerenciamento de contas de usuários (criação, atualização e exclusão).
Relação: Casos de uso relacionados ao “Realizar Login” por meio de <<extend>>.
Pré-condição: O usuário deve possuir permissões adequadas (administrador ou colaborador autenticado).

3.3 Responder Questionário de Felicidade — Colaborador

Descrição: O colaborador responde periodicamente ao questionário para registrar seu estado emocional.
Relação: Inclui o caso “Registrar Grau de Felicidade Anônimo” e pode se estender a “Participar de Gamificação” e “Enviar Sugestão”.
Fluxo Principal: O sistema exibe o questionário → o colaborador responde → os dados são salvos no histórico pessoal.

3.4 Registrar Grau de Felicidade Anônimo — Colaborador

Descrição: Permite o envio de um registro de felicidade sem identificação direta do colaborador.
Relação: É um caso <<include>> do questionário de felicidade.

3.5 Participar de Gamificação — Colaborador

Descrição: O colaborador acumula pontos por respostas e interações, participando de rankings e desafios.
Relação: Estende o caso “Responder Questionário de Felicidade”.
Pré-condição: Deve haver registros válidos de felicidade no sistema.

3.6 Enviar Sugestão — Colaborador

Descrição: Permite ao colaborador enviar sugestões de melhorias ou ações relacionadas ao ambiente de trabalho.
Relação: Estende o caso “Responder Questionário de Felicidade”.

3.7 Visualizar Histórico Pessoal — Colaborador

Descrição: Exibe ao colaborador seu histórico de registros de felicidade e evolução ao longo do tempo.
Pré-condição: O colaborador deve estar autenticado.

3.8 Visualizar Dashboard da Equipe — Gestor / Diretor

Descrição: Exibe indicadores agregados de felicidade dos colaboradores da equipe.
Fluxo Principal: O gestor ou diretor acessa o painel → o sistema processa e apresenta gráficos e médias.

3.9 Receber Sugestões — Gestor

Descrição: O gestor recebe e visualiza as sugestões enviadas pelos colaboradores para possíveis ações.
Pré-condição: Deve haver sugestões enviadas no sistema.

3.10 Gerenciar Usuários e Permissões — Administrador

Descrição: Permite ao administrador criar, editar ou remover contas e papéis de acesso.
Pré-condição: Usuário autenticado com permissão administrativa.

3.11 Configurar Integração com Ponto — Administrador

Descrição: Define parâmetros técnicos da integração com o sistema de ponto eletrônico.
Fluxo Principal: O administrador acessa as configurações → insere dados de integração → o sistema valida e salva.

3.12 Enviar Registro de Ponto — Sistema de Ponto (Externo) / Colaborador

Descrição:
Representa o momento em que o colaborador realiza a entrada na empresa, registrando o ponto por meio do Sistema de Ponto.
Esse evento aciona automaticamente o Termômetro da Felicidade, solicitando que o colaborador informe seu grau de felicidade.

## 4. Diagrama UML
![alt text](image-1.png)
