# 🧠 MVP – Análise de Dados e Boas Práticas | PUC-Rio

Este projeto faz parte do MVP da disciplina **Análise Exploratória e Pré-Processamento de Dados**, do curso de pós-graduação em Ciência de Dados da PUC-Rio.

---

## 📌 Objetivo

O objetivo é realizar uma análise exploratória e o pré-processamento completo de um dataset real, compreendendo:

- Entendimento e definição do problema
- Análise descritiva e visual dos dados
- Preparação dos dados para modelagem futura

---

## 📂 Dataset Utilizado

- **Fonte:** UCI Machine Learning Repository  
- **Dataset:** [Car Evaluation Data Set](https://archive.ics.uci.edu/dataset/19/car+evaluation)
- **Descrição:** Avaliação de carros com base em atributos como segurança, número de portas, preço de manutenção, entre outros.
- **Download no projeto:** [car.data.txt (versão raw)](https://raw.githubusercontent.com/Crlhju/MVP-Analise-de-Dados-PUC-RIO/refs/heads/main/car.data.txt)

---

## 🧱 Estrutura do Projeto

- `car.data.txt`: Arquivo com o dataset
- `MVP_Analise_de_dados.ipynb`: Notebook do Google Colab com todo o desenvolvimento

---

## 🧪 Etapas Realizadas no Notebook

1. **Definição do problema**  
   Analisamos como diferentes características de um carro influenciam sua classificação final (ótimo, aceitável, inaceitável).

2. **Importação e carregamento do dataset**  
   Utilizando a biblioteca `pandas`, carregamos os dados direto do GitHub com `read_csv()`.

3. **Criação de cópia de trabalho dos dados**  
   Uma versão do DataFrame original foi copiada para preservar os dados brutos e manipular à parte.

4. **Verificação de valores nulos e inconsistentes**  
   Confirmamos que não existem valores ausentes ou inválidos.

5. **Normalização textual dos dados**  
   Foi realizada a substituição dos códigos das variáveis por rótulos mais claros e descritivos.

6. **Visualizações individuais e combinadas**  
   Foram gerados diversos gráficos com `seaborn` para entender a distribuição dos atributos e sua relação com a variável-alvo.

7. **Resumo estatístico dos dados codificados**  
   Após codificação com `LabelEncoder`, geramos estatísticas descritivas para validar a consistência dos dados.

8. **Pré-processamento final dos dados**  
   Incluiu:
   - Codificação dos atributos categóricos
   - Normalização com `MinMaxScaler`
   - Divisão treino/teste (80/20) para futuros modelos

---

## 🛠️ Bibliotecas Utilizadas

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `sklearn.preprocessing`
- `sklearn.model_selection`

---

## ✅ Conclusões

- O atributo **segurança** (`safety`) mostrou maior influência sobre a classificação final do carro.
- Não foram encontrados dados faltantes.
- O dataset está balanceado em termos de estrutura, mas há **desequilíbrio nas classes**, com predominância da categoria `unacc`.
- O pré-processamento garantiu um conjunto de dados limpo, estruturado e pronto para futuros modelos de aprendizado supervisionado.

---

## 🔗 Link do notebook

- [Clique aqui para abrir no Google Colab](https://colab.research.google.com/drive/1bdLBkaP_tYEH8p5R6IrIwOsCgWNfgtmW?authuser=0#scrollTo=rnXaByIoD35R)

---

## 👨‍💻 Autor

**Juliano Faiolo**  
Aluno de Pós-graduação em Ciência de Dados – PUC-Rio  
[github.com/Crlhju](https://github.com/Crlhju)

