FROM rocker/rstudio-stable:latest
## Work-around to make Docker Hub use the Dockerfile 
## from https://github.com/rocker-org/rocker-versioned/tree/master/rstudio
WORKDIR /home/rstudio/data
COPY data/movies.csv movies.csv
COPY data/credits.csv credits.csv
