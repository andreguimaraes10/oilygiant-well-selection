# Seleção de Região para Desenvolvimento de Poços de Petróleo — OilyGiant

## Objetivo
Recomendar, com base em aprendizado de máquina e simulação estatística, 
a melhor região para a OilyGiant desenvolver novos poços de petróleo, 
maximizando o lucro e mantendo o risco de prejuízo abaixo de 2,5%.

## Contexto do Problema
A empresa avalia 3 regiões candidatas com 100.000 registros de poços 
cada. O orçamento disponível é de US$ 100 milhões para desenvolver 
200 poços por região, com receita de US$ 4.500 por mil barris extraídos.

## Metodologia
1. **Análise exploratória** dos dados das 3 regiões
2. **Modelagem preditiva** com Regressão Linear para estimar volume de reservas
3. **Comparação com modelo dummy** (baseline) para validar a utilidade do modelo
4. **Simulação de seleção de poços** — seleção dos 200 melhores entre 500 avaliados
5. **Análise de risco via Bootstrapping** com 1.000 reamostragens por região
6. **Recomendação final** com base em lucro médio esperado e risco de prejuízo

## Tecnologias
- Python
- Pandas
- NumPy
- Scikit-learn

## Resultado
A Região 1 foi recomendada como a mais adequada para investimento, 
sendo a única com risco de prejuízo inferior a 2,5% e maior lucro 
médio esperado entre as regiões aprovadas no critério de risco.
