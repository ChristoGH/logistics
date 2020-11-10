conda create --name logistics python=3.7



docker build -t datascience . 
<!-- This works: -->
docker run -it --rm datascience bash

sudo docker run -it --rm -v /media/lnr-ai/christo/github_repos/logistics:/datascience -p 8888:8888 datascience

sudo docker run -d -p 8787:8787 -w /home/user -v /media/lnr-ai/christo/github_repos/logistics:/home/rstudio -e PASSWORD=newPasswword rocker/rstudio

sudo docker run -d -p 8999:8787 -w /home/user -v /media/lnr-ai/christo/github_repos/sebastian:/home/rstudio -e PASSWORD=newPasswword rocker/rstudio