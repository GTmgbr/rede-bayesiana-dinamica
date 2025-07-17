# Previsão de Saúde do Solo com Redes Bayesianas Dinâmicas

Este projeto implementa uma **Rede Bayesiana Dinâmica (DBN)** para inferir a **saúde do solo agrícola** com base em observações semanais do aspecto visual das plantações, utilizando **Python** e a biblioteca `pgmpy`.

![Image](https://github.com/user-attachments/assets/6805eee2-6c89-4415-b50d-bebcd4e69bb7)

## 🧩 O que é uma Rede Bayesiana Dinâmica (DBN)

É um modelo probabilístico gráfico que representa **variáveis ao longo do tempo**, capturando suas **dependências temporais**.

Ela é uma extensão das Redes Bayesianas tradicionais, onde:

- Cada instante de tempo é representado por uma **cópia do modelo**, conectada ao próximo instante;
- As **variáveis ocultas** (como o estado real do solo) são inferidas a partir das **variáveis observáveis** (como o aspecto da cultura);
- As **transições entre estados** ao longo do tempo são modeladas probabilisticamente, permitindo prever e inferir comportamentos futuros.

As DBNs são amplamente usadas em problemas onde o estado do sistema evolui no tempo, como diagnósticos médicos, robótica, previsão de falhas, e, neste caso, agricultura de precisão.

## 🌾 Cenário

Uma fazenda com **200 talhões** precisa monitorar a **saúde do solo**, que pode ser rica, moderada ou pobre. Como análises químicas são caras, utiliza-se um **drone que fotografa semanalmente** os talhões e classifica o **aspecto da cultura** como vigorosa, amarelada ou murcha.

Essas observações visuais são indícios indiretos da saúde do solo. Como o solo evolui com o tempo, o problema é ideal para ser modelado com uma **Rede Bayesiana Dinâmica (DBN)**, que permite inferir o estado oculto do solo a partir do histórico de observações.

## 🎯 Objetivo

Construir uma **Rede Bayesiana Dinâmica (DBN)** para:

- **Inferir** a saúde real do solo a partir de observações históricas do aspecto da cultura;
- **Apoiar decisões** sobre uso de fertilizantes e práticas agrícolas;
- **Avaliar** o desempenho do modelo por meio de métricas de classificação.

## 🧠 Tecnologias Utilizadas

- Python
- [pgmpy](https://pgmpy.org/) – Modelagem de Redes Bayesianas Dinâmicas
- pandas, numpy – Manipulação de dados
- matplotlib – Visualizações
- scikit-learn – Divisão de dados e métricas de avaliação

