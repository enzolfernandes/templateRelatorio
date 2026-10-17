# Meu modelo de relatório em LaTeX — UNESP/FEIS

Organizei e utilizei este modelo durante minha graduação em Engenharia Elétrica na UNESP/FEIS. Ele reúne a estrutura de um relatório acadêmico, bibliografia e exemplos de conteúdo sobre circuitos e filtros.

![Logotipo da UNESP utilizado na capa](images/logoUNESP.jpg)

## Estrutura

| Arquivo | Conteúdo |
| --- | --- |
| [main.tex](main.tex) | Documento principal e pacotes |
| [0_capa.tex](0_capa.tex), [0_sumario.tex](0_sumario.tex) | Capa e sumário |
| `1_objetivos.tex` a `6_conclusao.tex` | Seções do relatório, com conteúdo de exemplo |
| [7_referencias.tex](7_referencias.tex), [bibliografia.bib](bibliografia.bib) | Referências via biblatex |
| [images](images) | Figuras utilizadas pelo exemplo |

## Preparar o documento

Com uma distribuição LaTeX que inclua os pacotes usados em `main.tex`, incluindo `biblatex-abnt`, e Biber disponíveis:

```shell
git clone https://github.com/enzolfernandes/templateRelatorio.git
cd templateRelatorio
pdflatex main.tex
biber main
pdflatex main.tex
pdflatex main.tex
```

Também é possível importar os arquivos em um editor LaTeX que ofereça esses pacotes e Biber. Substitua os dados da capa, o texto das seções, as imagens e as entradas bibliográficas pelos do seu trabalho. Os capítulos atuais contêm um relatório de exemplo, não apenas espaços em branco.

## Contexto e autoria

Meu [histórico](https://github.com/enzolfernandes/templateRelatorio/commits/master/) registra a organização, formatação e ajustes do material desde 2021. O estilo usa margens e referências próximas às convenções acadêmicas brasileiras; não é apresentado como modelo oficial ou certificação de conformidade da UNESP/ABNT. Confira as exigências da disciplina ou instituição.

As imagens e fontes bibliográficas conservam sua atribuição. O repositório contém a licença [GNU GPL v3](LICENSE). Esta revisão acrescentou instruções e navegação em 17/10/2026; não recompilou o documento.
