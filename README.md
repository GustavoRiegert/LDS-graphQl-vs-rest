# LDS-graphQl-vs-rest
Comparativo de Desempenho: GraphQL vs REST
Este projeto apresenta um estudo comparativo entre GraphQL e REST, analisando desempenho em três cenários distintos de consultas. A análise considera métricas como tempo de execução e tamanho dos payloads em um ambiente de teste configurado para garantir reprodutibilidade.

Objetivo
O objetivo do experimento é identificar as vantagens e limitações de cada abordagem em diferentes cenários de uso, auxiliando desenvolvedores na escolha da arquitetura mais adequada para suas necessidades.

Cenários Avaliados
Consultas Simples (Cenário 1):
Consultas que retornam dados pequenos e específicos, simulando buscas rápidas e diretas.

Consultas Complexas (Cenário 2):
Consultas que demandam retornos maiores e múltiplos relacionamentos, comuns em aplicações intermediárias.

Consultas Extensivas (Cenário 3):
Consultas que retornam um volume massivo de dados, simulando cenários extremos, como relatórios completos ou carregamento de dashboards.

Ambiente de Teste
Os testes foram realizados em uma instância Amazon EC2 t2.micro, configurada com:

1 vCPU
957 MiB de RAM
Sistema Operacional Ubuntu 24.04
Essa configuração foi escolhida para simular um ambiente leve e acessível, garantindo recursos suficientes para operações típicas de APIs.

Resultados
Os principais insights do estudo incluem:

GraphQL: Apresentou maior eficiência em cenários que demandam flexibilidade e consultas complexas, com menores tempos de execução e tamanho de payload.
REST: Mostrou-se robusto e eficiente em consultas simples, mas menos adaptável para cenários mais complexos devido ao envio de dados desnecessários.
Gráficos e métricas detalhadas estão disponíveis na seção de resultados do relatório.

Como Reproduzir
Configure uma instância Amazon EC2 com as especificações descritas.
Clone este repositório:
bash
Copiar código
git clone https://github.com/GustavoRiegert/LDS-graphQl-vs-rest.git
Instale as dependências e execute os scripts de teste conforme instruções nos arquivos do repositório.
Contribuições
Sugestões e melhorias são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.
