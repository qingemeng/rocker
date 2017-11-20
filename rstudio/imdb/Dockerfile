FROM rocker/rstudio-stable:latest
## Work-around to make Docker Hub use the Dockerfile 
## from https://github.com/rocker-org/rocker-versioned/tree/master/rstudio
WORKDIR /home/rstudio
COPY setup.R .
RUN apt-get update
RUN apt-get install libxml2-dev libssl-dev zlib1g-dev -y
RUN Rscript setup.R

CMD RUN git clone https://github.com/qingemeng/R_visualization_wwcode.git wwcode && chown rstudio:rstudio wwcode