# CE001

[![Build Status](https://travis-ci.org/leg-ufpr/ce001.svg?branch=master)](https://travis-ci.org/leg-ufpr/ce001)

## CE001 - Bioestatística

Repositório da disciplina CE001 - Bioestatística, ministrada na UFPR,
para diversos cursos de graduação.

Este repositório contém todo o material de aula e os arquivos
necessários para gerar a página da disciplina, disponível em:
http://cursos.leg.ufpr.br/ce001

### Para gerar o site

O site é todo construído usando apenas o [R Markdown][], por isso, o
código fonte está nos arquivos `Rmd`. Para gerar o site você precisará
das versões mais recentes dos pacotes `rmarkdown` e `knitr`.

1. Copie (clone ou fork) esse repositório
2. Apague o diretório `docs/`
3. Abra o R na raíz, carregue os pacotes e renderize o site com
   `render_site()`

```r
library(rmarkdown)
render_site()
```

### Licença

O conteúdo deste repositório, das páginas, e do material da disciplina
está está disponível por meio da [Licença Creative Commons 4.0][]
(Atribuição/NãoComercial/PartilhaIgual).

![Licença Creative Commons 4.0](img/CC_by-nc-sa_88x31.png)


[Licença Creative Commons 4.0]: https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt_BR
[R Markdown]: http://rmarkdown.rstudio.com
