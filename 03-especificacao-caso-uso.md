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

## 3.2 Cadastrar Conta
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Cadastrar Conta |
| **Ator Principal** | Colaborador / Administrador |
| **Pré-condições**  | Usuário autenticado com permissões adequadas |
| **Fluxo Principal**| 1. Usuário acessa tela de cadastro <br> 2. Preenche dados obrigatórios <br> 3. Sistema valida e cria a conta |
| **Fluxos Alternativos** | Dados inválidos → Sistema solicita correção |
| **Pós-condições**  | Conta criada com sucesso |

---

## 3.3 Editar Conta
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Editar Conta |
| **Ator Principal** | Colaborador / Administrador |
| **Pré-condições**  | Usuário autenticado |
| **Fluxo Principal**| 1. Usuário acessa sua conta <br> 2. Altera dados desejados <br> 3. Sistema valida e confirma alterações |
| **Fluxos Alternativos** | Dados inválidos → Sistema solicita correção |
| **Pós-condições**  | Dados atualizados com sucesso |

---

## 3.4 Excluir Conta
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Excluir Conta |
| **Ator Principal** | Administrador |
| **Pré-condições**  | Administrador autenticado |
| **Fluxo Principal**| 1. Administrador seleciona conta <br> 2. Sistema exibe confirmação <br> 3. Conta é removida do sistema |
| **Fluxos Alternativos** | Se usuário tentar excluir sua própria conta → Sistema bloqueia ação |
| **Pós-condições**  | Conta removida do sistema |

---

## 3.5 Responder Questionário de Felicidade
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

## 3.6 Registrar Grau de Felicidade Anônimo
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Registrar Grau de Felicidade Anônimo |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Acesso ao questionário ativo |
| **Fluxo Principal**| 1. Colaborador responde questionário <br> 2. Sistema salva resposta sem vínculo com identidade |
| **Pós-condições**  | Registro anônimo armazenado |
| **Relações**       | `<<include>> do Questionário de Felicidade` |

---

## 3.7 Participar de Gamificação
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Participar de Gamificação |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Respostas válidas no questionário |
| **Fluxo Principal**| 1. Colaborador participa respondendo <br> 2. Sistema gera pontos e atualiza ranking |
| **Pós-condições**  | Colaborador pontua na gamificação |
| **Relações**       | `<<extend>> do Questionário de Felicidade` |

---

## 3.8 Enviar Sugestão
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Enviar Sugestão |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Colaborador autenticado |
| **Fluxo Principal**| 1. Colaborador escreve sugestão <br> 2. Sistema registra e envia ao Gestor |
| **Pós-condições**  | Sugestão disponível para gestores |
| **Relações**       | `<<extend>> do Questionário de Felicidade` |

---

## 3.9 Visualizar Histórico Pessoal
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Visualizar Histórico Pessoal |
| **Ator Principal** | Colaborador |
| **Pré-condições**  | Colaborador autenticado |
| **Fluxo Principal**| 1. Colaborador acessa histórico <br> 2. Sistema exibe registros passados |
| **Pós-condições**  | Histórico exibido para análise individual |

---

## 3.10 Visualizar Dashboard da Equipe
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Visualizar Dashboard da Equipe |
| **Ator Principal** | Gestor / Diretor |
| **Pré-condições**  | Usuário autenticado |
| **Fluxo Principal**| 1. Usuário acessa dashboard <br> 2. Sistema processa e apresenta gráficos |
| **Pós-condições**  | Indicadores exibidos para tomada de decisão |

---

## 3.11 Receber Sugestões
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Receber Sugestões |
| **Ator Principal** | Gestor |
| **Pré-condições**  | Sugestões enviadas por colaboradores |
| **Fluxo Principal**| 1. Sistema lista sugestões <br> 2. Gestor visualiza e avalia |
| **Pós-condições**  | Sugestões ficam disponíveis para análise |

---

## 3.12 Gerenciar Usuários e Permissões
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Gerenciar Usuários e Permissões |
| **Ator Principal** | Administrador |
| **Pré-condições**  | Administrador autenticado |
| **Fluxo Principal**| 1. Administrador acessa painel de usuários <br> 2. Adiciona, altera ou remove permissões |
| **Pós-condições**  | Usuários e papéis atualizados |

---

## 3.13 Configurar Integração com Ponto
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Configurar Integração com Ponto |
| **Ator Principal** | Administrador |
| **Pré-condições**  | Administrador autenticado |
| **Fluxo Principal**| 1. Admin insere parâmetros técnicos <br> 2. Sistema valida <br> 3. Configuração salva |
| **Pós-condições**  | Integração habilitada |

---

## 3.14 Enviar Registro de Ponto
| Item               | Descrição |
|--------------------|-----------|
| **Nome**           | Enviar Registro de Ponto |
| **Ator Principal** | Sistema de Ponto (Externo) |
| **Pré-condições**  | Sistema de ponto ativo |
| **Fluxo Principal**| 1. Colaborador registra entrada <br> 2. Sistema de ponto envia dados ao Termômetro <br> 3. Sistema solicita grau de felicidade |
| **Pós-condições**  | Registro de ponto vinculado ao questionário de felicidade |
