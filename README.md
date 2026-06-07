# State of Data Brasil 2024 – Análise dos Fatores que Influenciam o Salário dos Profissionais de Dados

**Integrantes:** [Vithor Gabriel] e [Larissa Brandim]

## Dashboard Interativo

Dashboard desenvolvido no Google Looker Studio:

**Link:** [https://datastudio.google.com/reporting/f982cc9b-d86f-4f22-9a40-59aaf588a77e]

---

## Pergunta Central

**Quais fatores mais influenciam o salário de um profissional de dados no Brasil em 2024?**

De acordo com as análises realizadas, é percptível que a senioridade e o tempo de experiência dão os faores mais relevantes e associados aos salários dos profissionais de dados. Existe uma medida que é diretamente proporcional aos avanços de níveis, exemplo, Júnior ao pleno, sênior e especialista, dessa forma o salário aumente de acordo com o nível. Nessa mesma óptica, os profissionais que possuem mais anos atuando tendem a ocupar posições que exigem uma responsabilidade maior, logo apresentaram salários maiores que os demais.

Além da experiência, o cargo exercido também apresentou influência relevante na remuneração. Profissionais atuando como Engenheiros de Dados, Cientistas de Dados e cargos de liderança apresentaram salários médios superiores aos observados em funções mais operacionais. O domínio de múltiplas ferramentas e tecnologias também demonstrou relação positiva com os salários, sugerindo que profissionais com maior diversidade de competências técnicas tendem a ser mais valorizados pelo mercado.

Por outro prisma, diferenças salariais também foram encontradas entre grupos demográficos e regiões do país. Entretanto, essa diferenças devem ser olhadas com atenção, já que cada caso é um caso específico, já que por sua vez, podem estar associadas a fatores adicionais e isolados dos demais dados, como, experiência; senioridade; setor de atuação e porte da empresa. Então, os resultados indicam que a progressão profissional, a experiência acumulada e o cargo ocupado são os principais fatores associados aos maiores níveis de remuneração no mercado brasileiro de dados em 2024.

---

## Principais Decisões de Limpeza dos Dados

Antes da análise estatística, foram realizados procedimentos de tratamento e padronização dos dados para garantir maior qualidade e confiabilidade dos resultados.

### Conversão das Faixas Salariais

A variável salarial foi disponibilizada em formato textual, representada por intervalos de renda. Para permitir cálculos estatísticos, cada faixa foi convertida para seu ponto médio. Por exemplo:

* De R$ 4.001 a R$ 6.000 → R$ 5.000
* De R$ 8.001 a R$ 12.000 → R$ 10.000

Essa abordagem possibilitou o cálculo de médias, medianas, correlações e demais métricas analíticas.

### Renomeação de Colunas

O conjunto de dados possui nomes de colunas pouco intuitivos, como "1.b_genero" e "2.h_faixa_salarial". As principais variáveis utilizadas na análise foram renomeadas com base no dicionário oficial do dataset, tornando o código mais legível e de fácil manutenção.

### Tratamento das Ferramentas Utilizadas

As tecnologias utilizadas pelos profissionais são representadas por colunas binárias (0 e 1). Essas variáveis foram mantidas nesse formato e analisadas individualmente para identificar as ferramentas mais utilizadas pelos participantes.

### Dados Sensíveis

Os campos de gênero e raça/cor apresentavam respostas ausentes e registros do tipo "Prefiro não informar". Esses dados não foram imputados, pois a ausência de resposta representa uma escolha do participante e sua alteração poderia introduzir vieses na análise.

### Padronização de Cargos

Foram identificadas diferentes nomenclaturas para cargos equivalentes, como "Analista de Dados" e "Data Analyst". Esses registros foram padronizados por meio de um mapeamento manual para facilitar comparações entre funções semelhantes.

---

## Estrutura do Projeto

```text
nome1-nome2-state-of-data/
├── README.md
├── notebook/
│   └── nome1-nome2-analise.ipynb
├── relatorio/
│   └── nome1-nome2-relatorio.pdf
└── dados/
    └── README.md
```

---

## Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Looker Studio
* GitHub

---

## Fonte dos Dados

State of Data Brazil 2024–2025, realizado pela comunidade Data Hackers em parceria com a Bain & Company.

Dataset disponível em:

https://www.kaggle.com/datasets/datahackers/state-of-data-brazil-20242025

---

## Referências

* Documentação do Pandas
* Documentação do NumPy
* Documentação do Matplotlib
* Documentação do Seaborn
* Dicionário Oficial do State of Data Brasil 2024
* Material da disciplina Análise Avançada de Dados – UNIFSA

---

## Considerações Finais

Os resultados desta análise indicam que experiência profissional, senioridade e cargo exercido são os fatores com maior associação aos salários dos profissionais de dados no Brasil em 2024. Embora diferenças entre grupos e regiões tenham sido observadas, essas relações devem ser interpretadas considerando as limitações do conjunto de dados e os possíveis vieses presentes na pesquisa.
