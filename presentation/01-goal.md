# To start at the end

**The final replication package**

## Files {transition="fade"}

Contents of a package (context: FSRDC)

::::: {.columns}
:::: {.column width="60%"}

```{.bash}
README.md
README.pdf
code/
  fsrdc/
    01-prepare-data.R
    02-analyze-data.R
    03-create-disclosable-data.R
  public/
    04-create-tables.do
    05-create-figures.do
    06-create-intext.do
data/
  public/
    dist_cepii.dta
    usa_00010.dta
run.sh
```

::::
::::{.column width="40%"}

```{.bash}
data/
  confidential/
    lbd_2001.dta
    icf_2024.dta
```

::::
:::::

## Files {transition="fade" }

**All code**, whether used in RDC or not

::::: {.columns}
::::{.column width="60%"}


```{.bash code-line-numbers="3-11,16"}
README.md
README.pdf
code/
  fsrdc/
    01-prepare-data.R
    02-analyze-data.R
    03-create-disclosable-data.R
  public/
    04-create-tables.do
    05-create-figures.do
    06-create-intext.do
data/
  public/
    dist_cepii.dta
    usa_00010.dta
run.sh
```

::::
::::{.column width="40%"}

```{.bash}
data/
  confidential/
    lbd_2001.dta
    icf_2024.dta
```

::::
:::::


## Files {transition="fade" }

**All public data**, whether used in RDC or not

::::: {.columns}
::::{.column width="60%"}


```{.bash code-line-numbers="12-15"}
README.md
README.pdf
code/
  fsrdc/
    01-prepare-data.R
    02-analyze-data.R
    03-create-disclosable-data.R
  public/
    04-create-tables.do
    05-create-figures.do
    06-create-intext.do
data/
  public/
    dist_cepii.dta
    usa_00010.dta
run.sh
```

::::
::::{.column width="40%"}

```{.bash}
data/
  confidential/
    lbd_2001.dta
    icf_2024.dta
```

::::
:::::

## Files {transition="fade" }

**NONE of the confidential data** present in the RDC

::::: {.columns}
::::{.column width="60%"}


```{.bash code-line-numbers="1"}
README.md
README.pdf
code/
  fsrdc/
    01-prepare-data.R
    02-analyze-data.R
    03-create-disclosable-data.R
  public/
    04-create-tables.do
    05-create-figures.do
    06-create-intext.do
data/
  public/
    dist_cepii.dta
    usa_00010.dta
run.sh
```

::::
::::{.column width="40%"}

```{.bash code-line-numbers="1-4"}
data/
  confidential/
    lbd_2001.dta
    icf_2024.dta
```

::::
:::::

## Content

:::::: {.columns}

::::: {.column width="50%"}

Full description as per the [(template) README](https://social-science-data-editors.github.io/template_README/)

:::::

::::: {.column width="30%"} 
[![README](images/img-2021-11-08-2.png)](https://social-science-data-editors.github.io/template_README/)

:::::
::::::

