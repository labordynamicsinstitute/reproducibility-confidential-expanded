# Exercise 2

:::: {.columns}

::: {.column width="30%"}

:::

::: {.column width="40%"}

![](qrcode.png){width="350" height="350"}


:::

::: {.column width="30%"}

:::

::::


## Downloading data via code

## Easiest:

**Stata**

```{.stata}
use "$URL" , clear
```

## Why not?

- will it be there in two months? in 6 years?
- what if the internet connection is down?

## Easy:

**Stata**

```{.stata}
global URL "https://www.cepii.fr/distance/dist_cepii.dta"
copy "$URL" (outputfile), replace
```

**R**

```{.r}
download.file(url="$URL",destfile="(outputfile)")
```

## What if the internet dies?

Use caching of downloaded data.

```{.stata}
// ::::  Process only if data are present 

capture confirm  file "${datapath}/dist_cepii.dta"
if _rc == 0 {
    di in green "Data file is present, processing data"
} else { 
    di in red "Downloading data" 
    copy "$URL" "${datapath}/dist_cepii.dta", replace
}

//============ at this point, the data is available ======
// ::::  Process always 

use "${datapath}/dist_cepii.dta", clear
// do stuff....
```

## That was easy!

On to confidential data!
