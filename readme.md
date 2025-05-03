# Classificador de Flores com Modelos de IA

Esta aplicação é um exemplo interativo de classificação de flores usando múltiplos algoritmos de aprendizagem de máquina aplicados ao dataset Iris. A aplicação é construída com Python e Flask, e permite comparar o desempenho de diferentes modelos como KNN, Árvore de Decisão, K-Means e Rede Neural Artificial (RNA).

## Recursos Principais

- **Múltiplos Algoritmos de Classificação**:
  - K-Nearest Neighbors (KNN)
  - Árvore de Decisão
  - K-Means
  - Rede Neural Artificial (RNA)

- **Visualizações Avançadas**:
  - Matriz de confusão para avaliação de desempenho
  - Superfície de decisão para visualizar as fronteiras de classificação
  - Gráfico de importância de atributos (para árvores de decisão e random forest)
  - Comparação direta entre os diferentes modelos

- **Interface Moderna e Responsiva**:
  - Design com cards interativos
  - Layout responsivo adaptável a diferentes dispositivos
  - Exibição intuitiva de métricas e resultados

## Modelos de Machine Learning

A aplicação utiliza vários algoritmos de classificação para o dataset Iris:

### K-Nearest Neighbors (KNN)
Um algoritmo que classifica um ponto com base na classe da maioria dos seus k vizinhos mais próximos no espaço de características.

### Árvore de Decisão
Um modelo que cria uma estrutura semelhante a uma árvore onde cada nó interno representa uma decisão baseada em um atributo, cada ramo representa um resultado dessa decisão, e cada folha representa uma classe.

### K-Means
Um algoritmo de agrupamento (clustering) não supervisionado que foi adaptado para tarefas de classificação através de um mapeamento de clusters para classes.

### Rede Neural Artificial (RNA)
Um modelo inspirado no cérebro humano que consiste em camadas de neurônios artificiais interconectados, capaz de aprender padrões complexos nos dados.

## Prints do Sistema

| Versão Web | Versão Mobile (Responsiva) |
| --- | --- |
| ![Versão Web do Sistema](/static/prints-sistema/print-web.png) | ![Versão Mobile do Sistema](/static/prints-sistema/print-mobile.png) |

## Exemplos de Flores Iris

| Iris Setosa | Iris Versicolor | Iris Virginica |
| --- | --- | --- |
| ![Iris Setosa](/static/images/iris-setosa-example.png) | ![Iris Versicolor](/static/images/iris-versicolor-example.png) | ![Iris Virginica](/static/images/iris-virginica-example.png) |

## Pré-requisitos

- Python 3.x instalado
- Pip (gerenciador de pacotes do Python)

## Como Ambientar o Projeto

1. **Clone o repositório ou extraia os arquivos do projeto**  
   Certifique-se de que o diretório do projeto contenha, pelo menos:
   - `back.py`
   - `front.html` (dentro do diretório `templates`)
   - `requirements.txt` com as dependências necessárias

2. **Criar o ambiente virtual**

   No diretório do projeto, execute:
   ```bash
   python -m venv venv
   ```

3. **Ativar o ambiente virtual**

   - No Windows (PowerShell):
     ```bash
     .\venv\Scripts\Activate
     ```
   - No Linux/MacOS:
     ```bash
     source venv/bin/activate
     ```

4. **Instalar as dependências**

   Com o ambiente virtual ativo, execute:
   ```bash
   pip install -r requirements.txt
   ```

## Executando a Aplicação

Após instalar as dependências, inicie o servidor Flask executando:
```bash
python back.py
```

O servidor ficará disponível em [http://127.0.0.1:8080](http://127.0.0.1:8080). Abra este endereço em seu navegador para utilizar a aplicação.

## Estrutura do Projeto

A estrutura básica do projeto é a seguinte:

```
Classificador-Flores-IA/
├── templates/
│   └── front.html       # Interface do usuário (Front-end)
├── static/
│   ├── images/          # Imagens das flores Iris
│   └── prints-sistema/  # Capturas de tela da aplicação
├── venv/                # Ambiente virtual (gerado)
├── back.py              # Servidor e lógica de ML (Back-end)
├── requirements.txt     # Lista de dependências do projeto
└── README.md            # Este arquivo
```

## Uso da Aplicação

1. **Selecionar o Modelo**: Escolha entre KNN, Árvore de Decisão, K-Means ou RNA.
2. **Treinar o Modelo**: Clique em "Treinar Modelo" para iniciar o treinamento com o algoritmo selecionado.
3. **Testar o Modelo**: Clique em "Testar Modelo" para avaliar o desempenho e visualizar as métricas e gráficos.
4. **Comparar Modelos**: Clique em "Comparar Modelos" para ver uma tabela comparativa entre os diferentes algoritmos.
5. **Classificar Nova Flor**: Insira as medidas de uma nova amostra e clique em "Classificar" para obter a predição.

## Extensões e Melhorias Possíveis

- Adição de mais algoritmos de aprendizagem de máquina
- Implementação de ajuste automático de hiperparâmetros
- Suporte a outros conjuntos de dados
- Exportação de modelos treinados

---

Este projeto foi desenvolvido como atividade para a disciplina de Aprendizagem de Máquina na UFCA.
