# Automação de Registro e Acompanhamento de Erros de Software com n8n

**Papel:**

Atue como um especialista em n8n, automação de processos e desenvolvimento de software.

**Objetivo:**

Crie uma automação no n8n para registrar, classificar e acompanhar erros identificados durante o uso de um sistema de software, facilitando a comunicação entre os usuários e a equipe de desenvolvimento.

**Público:**

Analistas-programadores, desenvolvedores de software e equipes de suporte técnico.

**Ferramentas envolvidas:**

- Google Forms: formulário para registrar os erros encontrados.
- Google Sheets: armazenamento e acompanhamento das ocorrências.
- Gmail: envio de notificações ao desenvolvedor responsável.
- n8n: integração das ferramentas e execução do workflow.

**Fluxo:**

1. Receber uma nova ocorrência registrada por meio do Google Forms.
2. Validar os dados recebidos, verificando se os campos obrigatórios foram preenchidos.
3. Classificar a prioridade do erro de acordo com seu impacto:
   - Alta: erro que impede uma funcionalidade essencial do sistema.
   - Média: erro que prejudica uma funcionalidade, mas permite continuar utilizando o sistema.
   - Baixa: erro visual ou problema que não compromete as funcionalidades principais.
4. Registrar a ocorrência no Google Sheets, incluindo descrição, data, prioridade, responsável e status.
5. Enviar um e-mail ao desenvolvedor responsável, contendo os dados da ocorrência e sua prioridade.
6. Atualizar o registro com o status da notificação enviada.

**Regras:**

- Não processar ocorrências sem descrição do erro ou identificação do solicitante.
- Não enviar notificações quando o endereço de e-mail do responsável for inválido ou estiver ausente.
- Definir a prioridade com base no impacto informado no formulário.
- Registrar novas ocorrências com o status inicial "Pendente".
- Evitar o registro duplicado da mesma ocorrência, utilizando um identificador único quando disponível.
- Registrar eventuais falhas no processamento ou no envio de notificações.
- Não marcar uma notificação como enviada quando ocorrer uma falha no envio do e-mail.

**Resultado esperado:**

Explique quais nós do n8n devem ser utilizados, a função de cada nó, suas principais configurações e a lógica de funcionamento do workflow.

Apresente a sequência de execução e as conexões entre os nós, indicando como devem ser implementadas as validações, as condições de classificação, o registro das ocorrências e o tratamento de erros.

Inclua também um exemplo da estrutura do formulário e das colunas da planilha, além de demonstrar o funcionamento da automação com um exemplo de ocorrência válida e outro de ocorrência inválida.