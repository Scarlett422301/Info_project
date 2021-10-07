## My project

For my project, I will analyze the `CA_ED` data.

To analyze the data you will need to install some `R` packages. The required packages can be installed using `R` commands.

``` r
install_pkgs <- row.names(installed.packages())
pkgs <- c("ggplot2", "ggthemes", "dplyr", "skimr", "patchwork")
for(p in pkgs){
	if(!(p %in% install_pkgs)){
		install.packages(p)
	}
}
```

## Execute the analysis

To execute the analysis, from the project folder you can run 

``` bash
Rscript -e "rmarkdown::render('data_preprocessing.Rmd')"
```

This will create a file called `report.html` output in your directory that contains the results.
