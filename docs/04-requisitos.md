# Especificação de Requisitos — Sistema de Almoxarifado

## 1. Contexto

O sistema tem como objetivo auxiliar no gerenciamento de materiais de um almoxarifado, permitindo controlar o estoque, as solicitações de materiais e o acesso dos usuários.

## 2. Requisitos Funcionais (RF)
Comportamentos, funcionalidades e ações que o sistema deve executar.

| ID | Nome | Descrição | Prioridade |
| :--- | :--- | :--- | :--- |
| **RF01** | Consulta de disponibilidade de recurso | O sistema deve permitir que os funcionários consultem a disponibilidade das peças, ferramentas e materiais cadastrados no almoxarifado. | Alta |
| **RF02** | Solicitação de empréstimo de recursos | O sistema deve permitir que os funcionários solicitem o empréstimo de peças, ferramentas ou materiais disponíveis, registrando a solicitação e vinculando-a ao respectivo usuário e recurso. | Alta |
| **RF03** | Notificação de prazo de devolução | O sistema deve permitir o envio de notificações aos funcionários sobre os prazos de devolução dos recursos emprestados, visando auxiliar no cumprimento das datas estabelecidas. | Média |
| **RF04** | Consulta ao histórico de empréstimos | O sistema deve permitir que os funcionários consultem o histórico de seus empréstimos, contendo informações sobre os recursos utilizados e seus respectivos registros de empréstimo e devolução. | Média |
| **RF05** | Solicitação de renovação de empréstimo | O sistema deve permitir que os funcionários solicitem a renovação do prazo de um empréstimo por meio da aplicação, sem a necessidade de realizar a solicitação presencialmente. | Média |
| **RF06** | Cadastro de recursos | O sistema deve permitir que o gestor de recursos cadastre peças, ferramentas e materiais, incluindo as informações necessárias para sua identificação e controle no almoxarifado. | Alta |
| **RF07** | Registro de devolução e estado de conservação | O sistema deve permitir que o gestor de recursos registre a devolução de um recurso e informe seu estado de conservação, de modo a manter atualizadas sua disponibilidade e integridade. | Alta |
| **RF08** | Consulta de empréstimos em atraso | O sistema deve permitir que o gestor de recursos visualize os empréstimos cujo prazo de devolução tenha sido ultrapassado. | Alta |
| **RF09** | Geração de relatórios de utilização dos recursos | O sistema deve permitir que o gestor de recursos gere relatórios relacionados à utilização dos recursos, incluindo informações como os itens mais emprestados e o tempo médio de utilização. | Média |
| **RF10** | Gerenciamento de permissões de acesso | O sistema deve permitir que o administrador gerencie as permissões dos usuários e gestores, determinando o acesso às funcionalidades disponíveis de acordo com cada perfil. | Alta |

---

## 3. Requisitos Não Funcionais (RNF)
Critérios de qualidade, segurança, desempenho e restrições técnicas.

| ID | Categoria | Descrição | Critério de Aceite |
| :--- | :--- | :--- | :--- |
| **RNF01** | Usabilidade | O sistema deve apresentar uma interface simples, clara e intuitiva, permitindo que os funcionários realizem as principais operações sem necessidade de conhecimentos técnicos avançados. | Novos usuários devem conseguir realizar a solicitação de um recurso em até 2 minutos, sem consultar manuais de instrução. |
| **RNF02** | Desempenho | O sistema deve apresentar os resultados das consultas de disponibilidade e do histórico de empréstimos em até 3 segundos após a solicitação do usuário, considerando condições normais de funcionamento. | Em um cenário de teste com 30 usuários acessando simultaneamente as telas de consulta e histórico, 95% de todas as requisições bem-sucedidas devem retornar os dados exibidos na interface em um intervalo inferior a 3 segundos, medido através de ferramentas de auditoria de rede. |
| **RNF03** | Segurança e controle de acesso | O sistema deve implementar mecanismos de controle de acesso baseados no perfil do usuário, permitindo que cada usuário visualize e utilize somente as funcionalidades para as quais possui permissão. | Contas com perfil de funcionário devem ter os botões de cadastro e relatórios ocultos ou desabilitados, impedindo qualquer acesso não autorizado. |
| **RNF04** | Integridade dos dados | O sistema deve garantir a integridade dos dados relacionados aos recursos, empréstimos, devoluções e estados de conservação, evitando alterações ou exclusões não autorizadas. | O sistema deve registrar logs de auditoria para toda alteração de estado de conservação ou exclusão de registros. |
| **RNF05** | Disponibilidade | O sistema deve permanecer disponível durante o horário de funcionamento da oficina, possibilitando a realização das operações necessárias para o gerenciamento dos recursos. | O sistema deve garantir disponibilidade contínua durante o horário de atendimento do almoxarifado, sem quedas por falhas internas de aplicação. |