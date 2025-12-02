# corpo-polimerico-cma
Este repositório contém a análise dos dados obtidos em um ensaio de tração realizado em um corpo de prova metálico/polimérico (dependendo do material testado). A partir da planilha Excel exportada pela máquina de ensaios, foram calculadas as principais propriedades mecânicas do material:
	•	Módulo de Elasticidade (E)
	•	Limite de Escoamento (σₑ)
	•	Tensão Máxima / Resistência à Tração (σₘₐₓ)
	•	Tenacidade (Uₜ) – área total sob a curva tensão × deformação


* Objetivo do Experimento

O objetivo deste experimento é caracterizar o comportamento mecânico do material analisado por meio do ensaio de tração. A partir dos dados de força, deslocamento e geometria do corpo de prova, determinamos as propriedades fundamentais que descrevem sua rigidez, resistência e capacidade de absorver energia antes da fratura. Isso ajuda a desocbrir qual o material utilizado.

*  Dados Utilizados

Os cálculos foram realizados a partir da tabela Excel fornecida pela máquina de ensaio, contendo:
	•	Deslocamento (mm)
	•	Força (N)
	•	Tempo (s)
	•	Tensão calculada (MPa)
	•	Deformação calculada (mm)


Além disso, foram considerados os valores geométricos do corpo de prova polimérico, medidos pelo paquímetro:
	•	Área inicial da seção transversal (A₀)
	•	Comprimento inicial de referência (L₀)

*  Metodologia dos Cálculos

- Módulo de Elasticidade (E)

calculado a partir da região linear elástica da curva tensão × deformação.
	•	Aplicou-se um filtro para selecionar apenas os pontos onde o comportamento é linear.
	•	Realizou-se uma regressão linear para obter o coeficiente angular da reta, que corresponde a E.
	•	O E encontrado foi: 1,47 GPa (ou o valor obtido no seu cálculo).

Referência: Lei de Hooke σ = E·ε (Callister, Ciência e Engenharia de Materiais).


- Limite de Escoamento (σₑ)

O limite de escoamento foi determinado pelo critério adotado no relatório:
	•	Identificação do primeiro ponto em que o comportamento deixa de ser proporcional.
	•	Foi adotado o critério de desvio relativo > 0,5% em relação à reta elástica.
	•	O ponto correspondente à tensão desse instante é o σₑ.

 
 - Tensão Máxima (σₘₐₓ)

A tensão máxima corresponde ao maior valor de tensão registrado na curva:

\sigma_{\text{máx}} = \max(\sigma)

Física: indica a resistência máxima do material antes do início do estricamento (necking).

- Tenacidade (Uₜ)

A tenacidade representa a energia por unidade de volume absorvida pelo material até a fratura.

Foi obtida pela área total sob a curva tensão × deformação e usando o método numérico do trapézio 

Referências
	•	CALLISTER, W. D. Ciência e Engenharia de Materiais.
	•	ASTM E8 – Standard Test Methods for Tension Testing of Metallic Materials.
	•	Apostilas e notas de aula de Ciência dos Materiais.
