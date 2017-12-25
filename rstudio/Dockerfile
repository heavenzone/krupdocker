FROM rocker/rstudio:latest

RUN apt-get update -qq && apt-get -y --no-install-recommends install \
libxml2-dev \ 
libcairo2-dev \
libsqlite-dev \
libmariadbd-dev \
libmariadb-client-lgpl-dev \
libpq-dev \
libssh2-1-dev \
&& R -e "source('https://bioconductor.org/biocLite.R')" \
&& install2.r --error \
--deps TRUE \ 
tidyverse \
dplyr \
ggplot2 \ 
devtools \
formatR \
remotes \
selectr \
rticles \
blogdown \
bookdown \
bookdownplus \
caret \
C50 \
party \
adabag \
randomForest \
ensembleR \
forecast \
rvest \
XML \
xml2
