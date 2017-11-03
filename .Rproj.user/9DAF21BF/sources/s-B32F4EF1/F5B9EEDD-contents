install.packages('DSC2014Tutorial', repo = c('http://taiwanrusergroup.github.io/R-2014',  "http://cran.csie.ntu.edu.tw"), type = 'win.binary')
install.packages("installr"); require(installr) 
updateR()
# installing/loading the latest installr package:
install.packages("installr"); require(installr) #load / install+load installr
updateR()
#-----
library(DSC2014Tutorial)
slides("Basic")
slides("ETL1")
slides("ETL2")
slides("DataAnalysis")
slides("Visualization1")
slides("Visualization2")
slides("Visualization3")
#-----
deps <- available.packages("http://taiwanrusergroup.github.io/R/src/contrib")[1,"Suggests"]
pkgs <- strsplit(gsub("\\s", "", deps), ",")[[1]]
for(i in seq_along(pkgs)) {
  # You can change your favorite repository
  if (require(pkgs[i], character.only = TRUE)) next
  install.packages(pkgs[i], repo = "http://cran.csie.ntu.edu.tw")
}
