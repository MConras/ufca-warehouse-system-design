# Planejamento Inicial — Sistema de Almoxarifado

## 1. Product Backlog
O Product Backlog abaixo apresenta as *User Stories* (US) priorizadas, organizadas com base no valor de negócio e na necessidade imediata para o funcionamento do MVP (Produto Mínimo Viável).

| ID | User Story | Prioridade |
| :--- | :--- | :--- |
| **US01** | Como solicitante, desejo consultar a disponibilidade de um material em estoque. | Alta |
| **US02** | Como solicitante, desejo solicitar materiais pelo sistema. | Alta |
| **US03** | Como solicitante, desejo receber notificações sobre o status da minha solicitação. | Alta |
| **US06** | Como gestor do almoxarifado, desejo cadastrar novos materiais no sistema. | Alta |
| **US07** | Como gestor do almoxarifado, desejo registrar a entrada e saída de materiais. | Alta |
| **US08** | Como gestor do almoxarifado, desejo visualizar materiais com estoque baixo. | Alta |
| **US04** | Como solicitante, desejo visualizar meu histórico de solicitações. | Média |
| **US05** | Como solicitante, desejo cancelar uma solicitação de material. | Média |
| **US10** | Como administrador do sistema, desejo gerenciar as permissões dos usuários. | Média |
| **US09** | Como gestor do almoxarifado, desejo gerar relatórios de movimentação. | Baixa |

---

## 2. Metodologia de Trabalho (Kanban)
Para o gerenciamento e acompanhamento das atividades, adotou-se a metodologia **Kanban** por meio do painel digital integrado no *GitHub Projects*. O fluxo de trabalho foi estruturado nas seguintes etapas:

*   **Backlog:** Repositório central de todas as tarefas pendentes.
*   **In progress:** Atividades em execução ativa no momento.
*   **In review:** Etapa reservada para a validação, revisão de artefatos e controle de qualidade antes da conclusão oficial.
*   **Done:** Destino das entregas finalizadas e validadas.

---

## 3. Justificativa das Escolhas

*   **Estratégia Kanban:** A escolha pelo Kanban justifica-se pela necessidade de **flexibilidade e transparência visual**. Diferente de metodologias que exigem *Sprints* fixas, o Kanban permite ajustar o ritmo de entrega e visualizar o ciclo de vida de cada artefato da documentação em tempo real, o que é ideal para o atual estágio de desenvolvimento e modelagem do sistema.
*   **Priorização:** A priorização do Backlog seguiu o critério de **valor operacional**. As funcionalidades rotuladas como "Alta" prioridade são vitais para que o almoxarifado possa realizar o fluxo completo de "solicitação-empréstimo-devolução", enquanto as funcionalidades de suporte (relatórios, histórico, cancelamento) foram movidas para prioridades média e baixa, garantindo que o sistema seja funcional o mais rápido possível.