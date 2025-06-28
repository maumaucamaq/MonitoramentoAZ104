# MonitoramentoAZ104
Dicas sobre monitoramento AZ-104

Monitoramento é um item importante em qualquer área da TI, é por um monitoramento eficaz que teremos dados sobre a saúde do nosso ambiente, como está a entrega, o consumo e os custos relacionados a nossa infraestrutura.

Esse documento vai trazer um resumo para estudo para AZ-104 focando no monitoramento de máquinas virtuais no Azure

A ferramenta utilizada no Azure para monitoramento é o Azure Monitor, dentro dela alguns conceitos são importantes:
- Métricas armazenam dados numéricos de recursos monitorados em um banco de dados de série temporal. O banco de dados de métricas é criado automaticamente para cada assinatura do Azure.
- Os Logs do Azure Monitor coletam logs e dados de desempenho que podem ser recuperados e analisados de maneiras diferentes usando consultas de log.

Alguns recursos são usados para se aprofundar nessas métricas e logs:
- O Metrics Explorer é usado para analisar dados de métricas do Azure Monitor.
- Já para coletar dados de logs usamos o workspace do Log Analytics.
- E usamos o Log Analytics para analisar dados dos Logs do Azure Monitor.

Podemos criar alertas também que notificam você proativamente sobre condições críticas com base na telemetria coletada e, potencialmente, tentam executar medidas corretivas. Os alertas são gerados a partir de regras de alerta que definem os critérios para o alerta e a ação a ser tomada quando o alerta for disparado. Não há regras de alerta criadas por padrão no Azure Monitor (exceto as Regras de alerta de anomalias de falhas do Application Insights). Além de criar suas próprias opções, há várias opções para começar rapidamente com regras de alerta baseadas em condições predefinidas, e diferentes opções estão disponíveis para diferentes serviços do Azure. Este artigo descreve as diferentes opções para criar regras de alerta no Azure Monitor e onde você pode encontrar mais informações sobre cada opção.

No caso de Virtual machine podemos coletar métricas e logs de:
- O host da VM – estes dados se relacionam com a sessão do Hyper-V que gerencia os sistemas operacionais convidados e incluem informações sobre CPU, rede e utilização de disco.
- O convidado da VM – esses dados se relacionam com o sistema operacional e os aplicativos em execução dentro da máquina virtual.

  Os dados no nível do host fornecem uma compreensão do desempenho e da carga gerais da VM, enquanto os dados de nível de convidado fornecem visibilidade dos aplicativos, componentes e processos em execução no computador e seu desempenho e integridade. Por exemplo, caso esteja solucionando um problema de desempenho, poderá começar com métricas de host para visualizar qual VM está sob carga pesada e, em seguida, usar métricas de convidado para detalhar os detalhes do sistema operacional e do desempenho do aplicativo.

  
