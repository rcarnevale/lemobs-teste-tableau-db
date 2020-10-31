## Contagens de Partido por Categoria da Renúncia

select count(*)
from congressresign
where party = STRING-DO-PARTIDO and category = STRING-DA-CATEGORIA

## Contagem de Renúncias por Ano por Partido

select count(*)
from congressresign
where party = STRING-DO-PARTIDO and resignation_date between 'yyyy-01-01' and 'yyyy-01-31'

## Contagem de Renúncias por Categoria, separadas por Ano e Partido

select count(*)
from congressresign
where party = STRING-DO-PARTIDO and 
resignation_date between 'yyyy-01-01' and 'yyyy-01-31' and
category = STRING-DA-CATEGORIA