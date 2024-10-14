### **Desafio-Construindo-um-modelo-de-Regress-o-para-marketing**:

### **🚀 Desafio**:


### **Etapa 01: Análise Descritiva**

Primeiro, você verificará a presença de valores ausentes, dados duplicados e fornecerá uma análise descritiva básica das variáveis. Vamos em frente! ​


### **Resultados da Análise Descritiva:**

1. **Valores ausentes** : Nenhuma das colunas apresenta valores ausentes.
2. **Valores duplicados** : Não há dados duplicados no conjunto de dados.
3. **Análise descritiva** :
    - O valor médio de investimento no **YouTube** é 178,02, com um desvio padrão de 102,45.
    - O valor médio de investimento no **Facebook** é 27,67, com um desvio padrão de 17,91.
    - O investimento em **Jornal** tem uma média de 35,24, com um desvio padrão de 24,90.
    - As **vendas** têm uma média de 16,92, com um desvio padrão de 6,31.

Com isso, podemos concluir que o conjunto de dados está em boas condições para avançar para a próxima etapa.
### **Etapa 01) Análise Descritiva**

Vamos importar os dados, operar o conjunto de dados, verificar possíveis inconsistências e realizar uma análise estatística básica.

#### Passos:

1. Importar o conjunto de dados.
3. Explorar os tipos de dados, valores ausentes e dados duplicados.
4. Realizar uma análise descritiva das variáveis.


### Etapa 02: Análise Exploratória

#### Passos:

1. **Correlação entre variáveis** : Calcular a matriz de brilho para entender como as variáveis ​​se relacionam.
2. **Visualizações** : Gerar gráficos de dispersão (gráficos de dispersão) para visualizar as relações entre as variáveis ​​independentes (investimentos) e a variável dependente (vendas).
3. **Detecção de Outliers** : identificar possíveis outliers visualmente.
### Explicação:

1. **Matriz de Correlação** : A matriz de demonstração ( `MKT.corr()`) calcula o coeficiente de demonstração de Pearson entre todas as variáveis, o que nos permite entender as relações numéricas entre as variáveis.
    
    - Um valor próximo de 1 ou -1 indica uma forte brilho (positiva ou negativa), enquanto um valor próximo de 0 indica pouca ou nenhuma brilho.
    - Utilizamos um **mapa de calor** para visualizar facilmente as correlações entre variáveis.
2. **Gráficos de Dispersão (Scatter Plots)** :
    
    - Os gráficos de dispersão permitem visualizar a relação entre os investimentos (YouTube, Facebook e Jornal) e as vendas.
    - Isso ajuda a identificar se há uma relação linear ou outros padrões entre as variáveis.
    
    

3. **Gráficos de Dispersão** (continuação):
    
    - O uso de gráficos de dispersão nos permite visualizar há uma tendência linear entre as variáveis ​​independentes (investimentos no YouTube, Facebook e Jornal) e a variável dependente (vendas). Isso pode nos ajudar a decidir se a regressão linear será adequada para modelar esses dados.
        
    - Se houver um padrão linear claro, podemos supor que o aumento nos investimentos pode estar relacionado ao aumento nas vendas, o que é essencial para o modelo de regressão que construiremos na próxima etapa.
        
4. **Detecção de Outliers** :
    
    - Utilizamos gráficos de **boxplot** para verificar a presença de outliers. Um outlier é um valor que se distancia significativamente do restante dos dados e pode influenciar negativamente o modelo.
        
    - Os boxplots mostram a distribuição das variáveis ​​e ajudam a identificar se há valores muito fora do padrão, que poderiam ser removidos ou ajustados no processo de modelagem.
    -

###**Etapa 03: Modelagem** , vamos construir um modelo de **regressão linear** simples que seja capaz de prever o valor das vendas com base em nossos investimentos no YouTube, Facebook e Jornal. A regressão linear é uma técnica que modela a relação entre uma variável dependente (vendas) e uma ou mais variáveis ​​independentes (investimentos).

### Passos:

1. **Importar as bibliotecas de permissão** .
2. **Dividir os dados** em variáveis ​​dependentes e independentes.
3. **Dividir o conjunto de dados** em treino e teste.
4. **Treinar o modelo de regressão linear** .
5. **Avaliar o modelo** com análises como o erro quadrático médio (MSE) e o coeficiente de determinação (R2R2).

### Explicação:

1. **Importação das bibliotecas** :
    - `train_test_split`: Dividimos o conjunto de dados em treino e teste, garantindo que o modelo seja avaliado de forma justa.
    - `LinearRegression`: A função que cria o modelo de regressão linear.
    - `mean_squared_error`e


Na **Etapa 04: Calculando Predição** , usaremos o modelo de regressão linear treinado na **Etapa 03** para realizar soluções de vendas com base em novos valores de investimento em marketing (YouTube, Facebook e Jornal). Isso permitirá que uma empresa avalie o impacto de diferentes níveis de investimento em suas vendas.

### Passos:

1. **Definir novos valores de investimento** .
2. **Usar o modelo treinado para prever as vendas** com esses novos investimentos.
3. **Interpretar a abrangência** para entender como os investimentos impactantes em vendas.

### Explicação:

1. **Novos investimentos** :
    
    - Definimos novos valores de investimento no **YouTube** , **Facebook** e **Jornal** como exemplo para prever o impacto nas vendas.
    - Esses valores podem ser ajustados de acordo com o cenário ou orçamento que a empresa deseja testar.
2. **Previsão de vendas** :
    
    - Usamos o modelo de regressão treinado ( `model`) para prever as vendas com os novos valores de investimento usando a função `predict()`.
    - O resultado será o valor previsto de vendas com base nos valores de investimento fornecidos.
3. **Interpretação** :
    
    - A previsão nos dá uma estimativa de quais vendas a empresa pode esperar ao investir os valores fornecidos em suas campanhas de marketing.
    - Isso ajuda a empresa a entender como diferentes níveis de investimento impactam as vendas e a tomada de decisões de alocação de orçamento.

### Exemplo de saída:

Se a empresa investir **200** no YouTube, **50** no Facebook e **30** no Jornal, a previsão de vendas poderá ser algo como:


### **Conclusão**

Após realizar as etapas descritas no desafio, apresentamos alguns pontos importantes que podem orientar a empresa em suas decisões sobre investimentos em marketing:

1. ###  **Análise Descritiva** :
    
    - Observamos que o conjunto de dados estava completo, sem valores ausentes ou duplicados, e bem distribuído para análise.
    - As estatísticas descritivas mostraram variações específicas nos investimentos em YouTube, Facebook e Jornal, bem como nas vendas, ou que nos deram um ponto de partida sólido para entender o comportamento dos dados.

2.  ### **Análise Exploratória** :
    
    - Identificamos que os investimentos no **YouTube** e **Facebook** têm um brilho positivo significativo com as vendas, indicando que esses canais têm um impacto maior no retorno de vendas.
    - O investimento no **Jornal** mostrou uma clareza menor, o que indica que seu impacto nas vendas é mais limitado ou menos direto.
    - Além disso, a análise dos gráficos de dispersão reforçou a relação linear entre as variáveis ​​de investimento e as vendas, especialmente no caso de YouTube e Facebook.
3.  ### **Modelagem** :
    
    - Usamos uma **regressão linear** para modelar a relação entre os investimentos em marketing e as vendas. O modelo foi treinado com um bom desempenho, conforme indicado pelo coeficiente de determinação (R2R^2R2) que nos mostrou quão bem o modelo conseguiu explicar a variação nas vendas.
    - O modelo mostrou que é possível prever as vendas com base

4. ### **Previsão** :

- Usando o modelo de regressão linear, conseguimos gerar **soluções específicas** sobre o impacto de diferentes níveis de investimento em marketing. Por exemplo, as específicas indicam um **potencial de crescimento nas vendas** ao aumentar os investimentos no **YouTube** e **Facebook** , mostrando que esses canais têm maior influência no aumento das vendas.
- Essas opções oferecem à empresa uma **base sólida** para tomar **decisões estratégicas** , permitindo ajustar os investimentos em marketing de maneira mais eficiente e direcionada, maximizando o retorno sobre os investimentos em campanhas publicitárias.
