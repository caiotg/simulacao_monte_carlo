# Simulação de Monte Carlo

A simulação de Monte Carlo é uma técnica estatística que utiliza o método de amostragem aleatória para modelar incertezas e riscos. Ela recebe esse nome em referência ao famoso cassino de Monte Carlo, conhecido por jogos de azar e aleatoriedade.

# Fórmula Retornos Sintéticos

A fórmula dos retornos sintéticos é uma abordagem para simular retornos de ativos financeiros com base em seus parâmetros estatísticos, como média, desvio padrão e correlações. Ela é amplamente utilizada em simulações de Monte Carlo para criar cenários realistas e explorar diferentes possibilidades.

$$ Retornos_sintéticos = média_retornos + Rpdf × L $$

### onde:
* média_retornos = Média dos retornos.
* Rpdf = Matriz aleatória gerada por alguma função de densidade de probabilidade.
* L = Matriz triangular inferior proveniente de uma decomposição de Cholesky, usando como base a matriz de covariância dos dados originais.

# Rpdf (Random Number Probability Distribution Function)

A função Rpdf, ou Random Number Probability Distribution Function, é uma função utilizada para gerar variáveis aleatórias com distribuição específica. Em simulações de Monte Carlo, é comum utilizar a distribuição normal padrão, que é a distribuição de probabilidade com média zero e desvio padrão um. Essa função é fundamental para a geração dos retornos sintéticos na simulação.

# Decomposição de Cholesky

A decomposição de Cholesky é uma técnica utilizada para decompor uma matriz simétrica e definida positiva em um produto de uma matriz triangular inferior e sua transposta. Essa decomposição é utilizada para gerar correlações entre os retornos sintéticos de diferentes ativos.

# Utilidades

A partir das métricas obtidas na simulação de Monte Carlo, é possível calcular o VAR da carteira para diferentes intervalos de confiança e medir se o risco que você está correndo é compatível com o que você aguenta perder. No caso dessa carteira, uma queda de 24,87% está dentro dos 95% dos cenários mais possíveis de acontecer no próximo ano.
