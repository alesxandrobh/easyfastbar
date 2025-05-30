# Checklist de Implantação e Correções - EasyFastBar

## Login
- [x] Consulta usuário no banco e autenticação
- [x] Persistência de sessão/token
- [x] Indicador de status do banco de dados na tela de login
- [x] Exibição de logo da empresa na tela de login
- [x] Customização visual avançada

## Usuários & Permissões
- [x] Controle de acesso por nível (admin sistema, admin loja, gerente, atendente, caixa)
- [x] Atendente só vê e manipula seus próprios pedidos
- [x] Tela de configuração só acessível para admin sistema/loja
- [ ] CRUD completo de usuários (criar, editar, excluir usuários pelo frontend)
- [ ] Gerenciamento visual de níveis de acesso

## Configuração da Empresa
- [x] Página de configuração com dados da empresa (nome, endereço, CNPJ, telefone, logo, configs fiscais, configs banco)
- [x] Upload de logo
- [x] Endpoint backend para buscar/atualizar configs
- [ ] Persistência e uso real das configs fiscais e de banco no backend
- [ ] Validação e feedback visual detalhado

## Produtos & Estoque
- [x] Cadastro, edição, exclusão de produtos/estoque
- [x] Upload de imagem com validação de tamanho
- [x] Filtros especiais no cardápio (bebidas, Brahma, salgados)
- [x] Exibição correta dos nomes dos produtos nos pedidos
- [ ] Controle de estoque automático ao vender/baixar produto

## Mesas
- [x] Atendente só pode ocupar mesa livre
- [x] Só o responsável pode liberar a mesa
- [x] Status de mesa: livre, ocupada, aguardando pagamento
- [ ] Visualização de histórico de ocupação/liberação
- [ ] Feedback visual para ocupação/liberação negada

## Pedidos Restaurante
- [x] Atendente só vê e fecha conta dos próprios pedidos
- [x] Kanban/fases de acompanhamento dos pedidos (com e sem preparo)
- [x] Status extra: "fechar_conta" e "aguardando_pagamento"
- [x] Permite fechar conta e atualizar status da mesa
- [ ] Visualização de histórico de pedidos por mesa
- [ ] Relatórios de vendas e faturamento detalhados

## Dashboard & Estatísticas
- [x] Dashboard com estatísticas básicas (pedidos, faturamento, produtos mais vendidos)
- [ ] Gráficos e relatórios avançados

## Outras Seções
- [x] Locação: dashboard, KPIs, controle de artigos alugados
- [ ] Integração fiscal (NFe, SAT, etc)
- [ ] Configuração avançada de banco de dados pelo frontend

---

**Legenda:**
- [x] OK/Implementado
- [ ] Falta implementar/ajustar

Atualize este arquivo conforme evoluir o projeto!

# Checklist de Implantação

- [x] Upload de imagens em produtos/estoque corrigido e validado
- [x] Endpoints e queries SQL ajustados para estatísticas e produtos mais vendidos
- [x] Permissões: gerente tem acesso a todas as seções, atendente só vê e manipula seus próprios pedidos e mesas
- [x] Correção de exibição de mesas, dashboards e nomes de produtos nos pedidos
- [x] Warnings do MUI Grid v2 corrigidos
- [x] Correção de problemas de autenticação (token expirado)
- [x] Todas as rotas e queries usam nomes de colunas corretos
- [x] Campo cliente em novo pedido agora é opcional, com campos avulsos
- [x] Filtros especiais no cardápio (bebidas, Brahma, salgados) implementados
- [x] Layout dos cards de mesa melhorado, hover visual implementado
- [x] Kanban/fases de acompanhamento dos pedidos implementado (com e sem preparo)
- [x] Adicionado status "fechar_conta" e "aguardando_pagamento" para pedidos/mesas
- [x] Checklist de implantação criado em `CHECKLIST_IMPLANTACAO.md` e atualizado
- [x] Página de configuração da empresa criada, com upload de logo, campos fiscais e de banco
- [x] Tela de login modernizada: logo, background com imagem, responsividade, ícones, sem rolagem vertical
- [x] Backend: endpoints para configuração da empresa, healthcheck do banco, permissões por nível de acesso
- [x] Frontend: restrição de acesso à tela de configuração, ajuste visual e responsivo da tela de login, exibição correta de logo e background
- [x] Tela de login finalizada (layout compacto, sem rolagem, responsiva)

## PENDENTES
- CRUD completo de usuários (criar, editar, excluir pelo frontend)
- Gerenciamento visual de níveis de acesso
- Persistência e uso real das configs fiscais e de banco no backend
- Validação e feedback visual detalhado nas configs
- Controle de estoque automático ao vender/baixar produto
- Visualização de histórico de ocupação/liberação de mesas
- Feedback visual para ocupação/liberação negada
- Visualização de histórico de pedidos por mesa
- Relatórios de vendas e faturamento detalhados
- Gráficos e relatórios avançados no dashboard
- Integração fiscal (NFe, SAT, etc)
- Configuração avançada de banco de dados pelo frontend
