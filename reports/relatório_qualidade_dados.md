## Conclusão

A análise exploratória identificou problemas de qualidade de dados relacionados principalmente à consistência e à completude. Verificou-se a existência de múltiplas representações para valores semanticamente equivalentes de ausência de informação, incluindo variações ortográficas, diferenças de capitalização, presença ou ausência de acentuação e uso de códigos distintos (por exemplo, "NÃO SABE", "NAO SABE", "N/D", "NULL" e "SEM INFORMAÇÃO"). Tais ocorrências exigiram a padronização dos registros e a posterior conversão para valores ausentes (NaN), visando assegurar a consistência semântica e a correta avaliação da completude das variáveis.

## Colunas mais críticas

As que provavelmente exigirão maior esforço de saneamento:

Criticidade muito alta
Plain Text
municipio
municipio_da_vitima
sl_suspeito_municipio
sl_vitima_naturalizado_municipio
sl_suspeito_naturalizado_municipio

 
pais
pais_da_vitima
pais_do_suspeito

 
nacionalidade_da_vitima
suspeito_nacionalidade

 
relacao_vitima_suspeito

 
faixa_etaria_da_vitima

 
violacao

 
motivacao
Avaliação resumida por coluna

---

## Grupo de colunas|Consistência |Conformidade |Completude |Unicidademunicípio |Alto problema |Alto problema |Médio |Alto problema

país Alto Alto Médio Médio
nacionalidade Alto Alto Médio Médio
naturalidade Alto Alto Médio Médio
relação vítima-suspeito Alto Médio Baixo Alto
faixa etária Alto Médio Médio Alto
motivação Médio Alto Baixo Médio
violação Médio Alto Baixo Médio
profissão Médio Médio Médio Médio
religião Médio Médio Médio Médio
etnia Baixo Médio Médio Baixo
gênero Baixo Baixo Médio Baixo
raça/cor Baixo Baixo Médio Baixo
Conclusão metodológica

Com base nos exemplos apresentados, a dimensão mais comprometida no dataset é Consistência, seguida por Conformidade e Unicidade. A principal causa é a coexistência de múltiplas representações para o mesmo conceito (municípios, países, nacionalidades, relações e faixas etárias), indicando ausência de padronização dos domínios de valores. Já a Completude é afetada pela ampla presença de categorias equivalentes a ausência de informação ("não sabe", "não informado", "nulo", etc.), que mascaram valores faltantes reais e exigem tratamento prévio antes das análises estatísticas ou de machine learning.
