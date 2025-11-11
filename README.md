C - Culture

# Pontos de atrito

1. Sistema LEGADO em Delphi mantido por um único desenvolvedor.
    - Concentração de conhecimento e criação de dependência em uma pessoa (síndrome da pessoa herói)
2. Problemas de escalabilidade e desempenho no time de operações.
    - Pode gerar problemas futuramente devido ao resultado que o cliente vai ter.
3. Novas features são enviadas diretamente para produção.
    - Por não passar por um ambiente de teste primeiro as probabilidade de ter um erro em produção aumenta
4. Deploy realizado manualmente.
    - Tarefa penosa, faz com que gaste tempo em uma tarefa que devia ser realizada de forma automatica
5. Monitoramento e testes iniciados apenas após o deploy.
    - Como os testes são iniciados apenas após o deploy a chance de parar o processo ou do cliente se deparar com o erro é muito grande, além é claro da questão do monitoramento que também poderia identificar erros e gargalos antes de estarem em ambiente de produção
6. Alto número de incidentes e muito tempo de recuperação, com demora para identificar e corrigir as causas.
    - Resultado de operação realizadas de maneira errônea e sem cuidado o suficiente, acaba gerando muitos erros em produção que o próprio cliente vai se deparar, também por conta da falta de uma fase de testes mais concreta e falta de monitoramento há uma grande demora para identificar e para corrigir os erros.

A - Automação

# Soluções de automação

1. Deploy realizado manualmente.
2. Utilizar praticas de CI/CD, assim garantindo que o código dos desenvolvedor passe por etapas cruciais para sua integridade e eficácia, além de diminuir o trabalho penoso de ter que subir manualmente todas as novas features, melhorias e correções assim diminuindo também a chance de erros.

# Plano de ação

1. Fomentar a cultura DevOps para que haja colaboração entre os times de desenvolvimento e operação, todos precisam confiar no processo.
2. Escolher uma ferramenta como Jenkins, GitLab CI/CD, GitHub Actions que automatizam desde a integração até a entrega.
3. Um repositório com controle de versão, como o GitHub, que vai acionar a pipeline de CI/CD a cada novo commit.
4. Implementar testes abrangentes, teste unitários, integração, e2e.
5. Garantir que os testes reflitam um ambiente de produção real.
6. Começar com pequenos passos e depois evoluir para estruturas mais robustas.
7. Manutenções regulares, a pipeline precisa de ajustes contínuos para se adaptar as mudanças do projeto.
8. Automatizar o Deploy, se possível com uma pré aprovação antes de ir ao ar.


L - Lean

# Solução Rápida e de grande valor
1. Identificar quais tarefas a serem feitas são prioritárias para o cliente.
2. Identificar em equipe a complexidade das tarefas anterior ao desenvolvimento.
3. Identificar o tempo que levaria para que cada tarefa seja realizada.
4. Priorizar tarefas mais simples e que entregam mais valor ao cliente.

M - Métricas

# Métricas de eficácia da automação

1. O tempo médio para a entrega do código e o deploy
    - Mostra a eficácia da automatização ao integrar e colocar as mudanças no ar.
2. Tempo médio para a resolução dos erros
    - Mostra a eficácia dos testes de maneira abrangente.
3. O número de incidentes
    - Mostra como mais etapas de segurança como as etapas de teste e de confirmação pré produção podem ajudar a evitar uma quantidade grande de erros.
4. Número de exceções não capturadas pela automação
    - Diz quantas vezes a automação falhou em capturar possíveis comportamento assim indicando pontos de melhoria na automação.
5. Número de horas trabalhadas
    - Pode ser um indicativo já que agora parte do time não perde mais tempo trabalhando em tarefas penosas.


S - Sharing

# Disseminar o conheciment
1. Promover cultura colaborativa, fazendo com que operações trabalhe em conjunto com desenvolvimento.
2. Treinamentos, onde os colaboradores mais experientes podem ensinar os novos colaboradores.
3. Treinamentos entre áreas. (operações para dev e dev para operações).
4. Analise pós ação, sessões de analise em grupo após grandes incidentes.
5. Documentação atualizada e acessivel sobre sistemas




