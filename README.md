# UWine: Clube de Vinhos da UVV

Projeto de conclusão de curso de Ciência de Dados da Universidade Vila Velha (UVV).
Autor: Aridalton de Sousa Moreira Júnior

## Parte 1: tamanho ideal da amostra

A base tem 1.120.000 notas fiscais e recebe cerca de 5.000 notas novas por dia, por isso foi tratada como população infinita. O objetivo desta parte é definir o tamanho ideal da amostra para estimar o gasto do cliente (TOTAL em reais), estratificando por tipo de conta (ESSENTIAL, VIP e PRIME).

### Etapas
- **A1.1:** tamanho ideal pela estabilização do erro-padrão (procedimento empírico prático por grupo e alocação de Neyman), com análise bootstrap.
- **A1.2:** análise e remoção de outliers por estrato (IQR), recálculo do tamanho ideal e efeito da entrada diária de notas.
- **A1.3:** testes de hipóteses entre duas amostras: normalidade (Anderson-Darling), independência, mesma distribuição e médias amostrais, com 1.000 sorteios bootstrap.
- **A2:** estatística descritiva das variáveis quantitativas e qualitativas.
- **A3:** pesquisa de satisfação em escala de 5 níveis, no geral e por sexo, com intervalos de confiança por bootstrap.

### Principais resultados
- Tamanho ideal da amostra: **5.400 notas fiscais** (cerca de 1,1 dia de entrada de notas).
- A estratificação de Neyman reduz o erro-padrão em cerca de 60% em relação à amostra aleatória simples.
- Duas amostras de 5.400 notas são independentes, têm a mesma distribuição e a mesma média.
- 80,7% dos clientes estão satisfeitos ou muito satisfeitos, com diferença significativa entre mulheres (76,6%) e homens (81,3%).

## Arquivos
- `WORKFLOW_PARTE_1.ipynb`: notebook com o código e os resultados.
- `ARIDALTON_JUNIOR.html`: versão em HTML do notebook executado.

## Como executar
1. Abra o notebook no Google Colab pelo botão "Open in Colab".
2. Faça o upload do arquivo `table4.csv` na pasta de arquivos do Colab. A base não está no repositório porque tem cerca de 400 MB, acima do limite do GitHub; ela é fornecida pelo professor da disciplina.
3. Execute: Ambiente de execução > Executar tudo.

## Vídeo de apresentação
[(link do YouTube)](https://www.youtube.com/watch?v=2UGDNatjmSE)
