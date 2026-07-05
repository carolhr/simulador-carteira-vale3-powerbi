# simulador-carteira-vale3-powerbi
# 📈 Simulador de Carteira e Análise de Risco (VALE3): Python + Power BI + Figma

<img width="1292" height="568" alt="Simulador" src="https://github.com/user-attachments/assets/c5eb5045-9fd8-4c18-8c04-dbcd1a523d8d" />


## 📌 Sobre o Projeto
Este repositório contém uma solução de Business Intelligence voltada para o mercado financeiro. O projeto simula uma carteira de investimentos ativa nas ações da Vale (VALE3) e calcula a volatilidade e o estresse do ativo através do conceito de Drawdown Máximo, cobrindo uma série histórica real de 5 anos.

## 🛠️ Arquitetura de Solução e Tecnologias
* **Engenharia de Dados (Python):** Script automatizado para extração, limpeza e modelagem inicial do histórico diário de cotações em formato tabular.
* **UI/UX Design (Figma):** Prototipagem da interface no estilo *Light Mode / Executive Wealth*, aplicando conceitos de respiro visual, hierarquia geométrica e sombras sutis para uma leitura analítica limpa.
* **Data Analytics (Power BI):** Desenvolvimento do motor de cálculo dinâmico (DAX) e integração com parâmetros de entrada numérica para simulação do usuário final.

## 🧮 Lógica de Negócios e Fórmulas Desenvolvidas (DAX)
O projeto se destaca pelo uso de variáveis (`VAR`) e inteligência analítica de dados:
* **Preço Atual:** Captura de forma automatizada o último fechamento de mercado disponível baseado no maior indexador de data.
* **Simulador de Aportes:** Cruzamento dinâmico entre os parâmetros digitados pelo usuário (Quantidade de Ações vs Preço Médio) para retornar o *Valor Investido*, *Patrimônio Atual* e o *Lucro/Prejuízo Nominal*.
* **Drawdown Máximo (Análise de Risco):** Fórmula matemática avançada que calcula o maior pico histórico do preço do ativo até a data corrente e o compara com o valor do dia atual, mapeando o percentual de estresse e risco de queda em um gráfico de áreas.
  
## markdown## 🐍 Como Executar o Script Python
O script de extração automatizada (`extract_vale3.py`) foi desenvolvido utilizando as seguintes bibliotecas principais:
* `yfinance` (para comunicação direta com as APIs do Yahoo Finance)
* `pandas` (para tratamento de dados estruturados)
* `openpyxl` (para exportação limpa em formato Excel)

Para rodar a extração localmente, basta instalar as dependências e executar o arquivo:
```bash
pip install yfinance pandas openpyxl
python extract_vale3.py

💡 *Projeto desenvolvido para fins de portfólio técnico de análise e engenharia de dados.*

