# Introdução ao Tidyverse

## Capítulo 1º

Vamos aprender filter(), pipe (%>%), arrange(), mutate()

- Para usar o filter() podemos fazer:

gapminder %>%

  filter(year == 2007, country == "United States")

- Para usar o arrange (ordernar do menor para o maior - colunas) e se quiser do maior para o menor usamos desc:

gapminder %>%

  arrange(gpdPercap)
  
- Em ordem decrescente:

gapminder %>%

  arrange(desc(gpdPercap))

- Vejamos um exemplo que usamos filter() e arrange() juntos:

gapminder %>%

  filter( year == 2007 ) %>%
  
  arrange(desc(gdpPercap))
  
- Agora que já sabemos usar o filter() e arrange (), vamos aprender a usar o mutate(). Vale lembrar que o mutate adiciona uma nova variável:

 
