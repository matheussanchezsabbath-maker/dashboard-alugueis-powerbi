[README_powerbi.md](https://github.com/user-attachments/files/29270779/README_powerbi.md)
# 🏠 Dashboard de Aluguéis no Brasil — Power BI

Dashboard interativo que analisa o mercado de aluguéis em cinco grandes cidades brasileiras, construído no **Power BI** — da limpeza dos dados (Power Query) à modelagem (DAX) e ao design final.

> 📍 Cidades analisadas: São Paulo, Rio de Janeiro, Belo Horizonte, Porto Alegre e Campinas · Dados de 2020.

---

## 🎯 Objetivo

Entender como variam os preços de aluguel de acordo com **cidade, área, número de cômodos, mobília e custos extras (condomínio, IPTU, seguro)** — e responder, com dados, onde e por que morar custa mais.

---

## 🔍 Principais descobertas

- **O aluguel é enviesado:** a média (R$ 3.896) fica bem acima da mediana (R$ 2.660), porque um grupo de imóveis de luxo puxa a média pra cima. A mediana representa melhor o aluguel "típico".
- **Plot twist do preço por m²:** São Paulo tem o maior aluguel absoluto, mas o **Rio de Janeiro é o mais caro por metro quadrado** (R$ 31/m² contra R$ 21/m² de Belo Horizonte).
- **O caso de Belo Horizonte:** BH tem aluguel total alto porque os imóveis são maiores — mas também concentra a **maior fatia de condomínio**, chegando a ~37% do custo total de morar (contra 16–23% nas outras cidades).
- **O aluguel não é o custo real:** somando condomínio, IPTU e seguro, o gasto mensal fica bem acima do valor "de vitrine".

---

## 🛠️ Etapas e técnicas

1. **Limpeza e transformação (Power Query):** correção de tipos, tratamento de valores faltantes (coluna de andar), remoção de outliers de área e decisão consciente sobre duplicatas.
2. **Modelagem (DAX):** criação de medidas (`AVERAGE`, `MEDIAN`, `COUNTROWS`, `DIVIDE`) e de uma coluna calculada de faixa de preço com `SWITCH`.
3. **Geolocalização:** categorização da coluna de cidade para uso em mapa de bolhas.
4. **Visualização:** cartões (KPIs), mapa, rankings, histograma, rosca de segmentação e gráficos de composição de custo.
5. **Design:** tema de cores personalizado, cabeçalho, e organização em múltiplas páginas com navegação consistente.

---

## 💻 Tecnologias utilizadas

- **Power BI Desktop**
- **Power Query** (limpeza e transformação)
- **DAX** (medidas e colunas calculadas)

---

## 📂 Estrutura do repositório

```
├── dashboard-alugueis.pbix   # arquivo do Power BI (abra no Power BI Desktop)
├── imagens/                  # prints das páginas do dashboard
└── README.md                 # este arquivo
```

> 💡 O arquivo `.pbix` pode ser aberto no Power BI Desktop (gratuito) para explorar o dashboard interativo.

---

## 📊 Sobre os dados

- **Fonte:** Brazilian Houses to Rent (Kaggle)
- **Conteúdo:** características de imóveis para aluguel (área, cômodos, cidade, custos) em cinco cidades brasileiras.
- **Recorte:** análise limitada às cinco cidades presentes na base, com dados de 2020.

---

## 👤 Autor

**Matheus Mucci Sanchez**
[LinkedIn](https://www.linkedin.com/in/matheus-mucci-sanchez-aaba72385/) · [GitHub](https://github.com/matheussanchezsabbath-maker)
