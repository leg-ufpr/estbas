# estbas

[![Build Status](https://travis-ci.org/leg-ufpr/estbas.svg?branch=master)](https://travis-ci.org/leg-ufpr/estbas)

## Estatística Básica

Repositório das disciplinas de Estatística Básica (CE00X), ministradas
na UFPR, para diversos cursos de graduação.

Este repositório contém todo o material de aula e os arquivos
necessários para gerar a página da disciplina, disponível em:
http://cursos.leg.ufpr.br/estbas

### Para gerar o site

O site é todo construído usando apenas o [R Markdown][], por isso, o
código fonte está nos arquivos `Rmd`. Para gerar o site você precisará
das versões mais recentes dos pacotes `rmarkdown` e `knitr`.

1. Copie (clone ou fork) esse repositório
2. Abra o R na raíz, carregue os pacotes e renderize o site com
   `render_site()`

```r
library(rmarkdown)
render_site()
```

**Observações**:

- Os slides são gerados individualmente, a partir dos arquivos fonte
  `Rmd`, disponíveis no diretório [slides](./slides).
- A publicação no site é automatizada através do
  [Travis](https://travis-ci.org). Os arquivos para essa automatização
  são [.travis.yml](./.travis.yml) (configura o build como se fosse um
  pacote do R), [_build.sh](./_build.sh) (roda o **rmarkdown**) na raíz
  do site, e [_deploy.sh](./_deploy.sh) (clona e gera o site diretamente
  no branch *gh-pages*).

### Licença

O conteúdo deste repositório, das páginas, e do material da disciplina
está está disponível por meio da [Licença Creative Commons 4.0][]
(Atribuição/NãoComercial/PartilhaIgual).

![Licença Creative Commons 4.0](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)


[Licença Creative Commons 4.0]: https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt_BR
[R Markdown]: http://rmarkdown.rstudio.com
