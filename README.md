# Analise_comportamento_usuario_teste_AAB
Projeto 9 -  Análise do comportamentos usuários no aplicativo com Teste A/A/B


# Descrição dos dados
 - Cada entrada de diário é uma ação do usuário ou um evento.
  - EventName — nome do evento
  - DeviceIDHash — dentificador de usuário exclusivo
  - EventTimestamp — hora do evento
  - ExpId — número do experimento: 246 e 247 são os grupos de controle, 248 é o grupo de teste

# Execução do Projeto

## Estude e verifique os dados
  - Quantos eventos ficam nos diários?
  - Quantos usuários ficam nos diários?
  - Qual é o número médio de eventos por usuário?
  - Qual é o período de tempo que os dados cobrem? Encontre a data máxima e mínima. Desenhe um histograma por data e hora. Você pode ter certeza de que possui os dados igualmente completos para todo o período? Os eventos mais antigos podem acabar aparecendo nos diários de alguns usuários por motivos técnicos, e isso pode distorcer o quadro geral.
  - Encontre o momento em que os dados começam a ser completos e ignore a seção anterior. Qual período os dados realmente representam?
  - Você perdeu muitos eventos e usuários ao excluir os dados mais antigos?
  - Certifique-se de ter usuários de todos os três grupos experimentais.
## Estude o funil de eventos
  - Veja quais eventos estão nos diários e sua frequência de ocorrência. Classifique-os por frequência.
  - Encontre o número de usuários que executaram cada uma dessas ações. Ordene os eventos pelo número de usuários. Calcule a proporção de usuários que executaram a ação pelo menos uma vez.
  - Em que ordem você acha que as ações ocorreram. Todos eles fazem parte de uma única sequência? Você não precisa levá-los em consideração ao calcular o funil.
  - Use o funil de eventos para encontrar a parcela de usuários que passam de uma etapa para a próxima. (Por exemplo, para a sequência de eventos A → B → C, calcule a proporção de usuários na etapa B para o número de usuários na etapa A e a proporção de usuários na etapa C para o número na etapa B.)
  - Em qual fase você perde mais usuários?
  - Qual é a parcela de usuários que faz o caminho inteiro, desde o primeiro evento até o pagamento?
## Estude os resultados do experimento
  - Quantos usuários há em cada grupo?
  - Temos dois grupos de controle no teste A/A, no qual verificamos nossos mecanismos e cálculos. Veja se há uma diferença estatisticamente significativa entre as amostragens 246 e 247.
  - Selecione o evento mais popular. Em cada um dos grupos de controle, encontre o número de usuários que realizaram essa ação. Encontre a proporção deles. Verifique se a diferença entre os grupos é estatisticamente significativa. Repita o procedimento para todos os outros eventos (economizará tempo se você criar uma função especial para este teste). Você pode confirmar se os grupos foram divididos corretamente?
  - Faça a mesma coisa para o grupo com fontes alteradas. Compare os resultados com os de cada um dos grupos de controle para cada evento isoladamente. Compare os resultados com os resultados combinados para os grupos de controle. Quais conclusões você pode tirar do experimento?
  - Qual nível de significância você definiu para testar as hipóteses estatísticas mencionadas acima? Calcule quantos testes de hipóteses estatísticas você realizou. Com um nível de significância estatística de 0,1, um de cada 10 resultados pode ser falso. Qual deveria ser o nível de significância?Se você quiser alterá-lo, execute as etapas anteriores novamente e verifique suas conclusões.
