Objetivo
Explorar o uso de uma LLM para apoiar a criação de casos de teste de integração em um sistema de cadastro de usuários, composto por front-end, API REST e banco de dados.

Prompt 1 – Geração de cenários de integração
Objetivo: gerar casos de teste para validar a comunicação entre Agent e API.
Prompt:
  Você é um Analista de QA Sênior especializado em testes de integração. Considere uma arquitetura composta por um Agent instalado no terminal POS que consome uma API REST. Gere casos de teste de integração cobrindo fluxo de sucesso, autenticação, atualização de configuração, falhas de comunicação, retentativas e persistência no banco de dados. Apresente os casos de teste contendo ID, objetivo, pré-condições, passos, dados de entrada e resultado esperado.

Prompt 2 – Geração de cenários de erro e resiliência
Objetivo: identificar falhas na integração e comportamentos inesperados.
Prompt:
  Você é um especialista em testes de integração e confiabilidade de sistemas distribuídos. Gere casos de teste para validar timeout, indisponibilidade da API, respostas HTTP inválidas, erros de autenticação, perda de conexão, duplicidade de mensagens e falhas de persistência. Considere os impactos na API, Agent e banco de dados.

Resultados obtidos
O primeiro prompt gerou cenários mais focados no fluxo funcional da integração, cobrindo comunicação entre Agent, API e banco de dados, com boa organização e rastreabilidade dos testes.
O segundo prompt ampliou significativamente a diversidade dos cenários, incluindo situações de falha, recuperação, retentativas automáticas, perda de conectividade e consistência de dados. Esses casos ajudaram a identificar cenários que não haviam sido considerados inicialmente.

Ajustes realizados nos prompts
Para melhorar os resultados foi necessário:
Definir claramente o papel do modelo como especialista em QA.
Informar a arquitetura envolvida e os componentes participantes.
Especificar o formato desejado dos casos de teste.
Solicitar explicitamente cenários negativos e de recuperação.
Orientar a IA a não assumir regras de negócio não informadas.
