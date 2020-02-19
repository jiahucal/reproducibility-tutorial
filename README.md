# reproducibility-tutorial
tutorial from FOSS2020
    1  cd /scratch
    2  df -h
    3  git clone https://github.com/jiahucal/reproducibility-tutorial.git
    4  ls
    5  clear
    6  wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
    7  bash Miniconda3-latest-Linux-x86_64.sh -b -p /opt/conda
    8  ln -s /opt/conda/pkgs/*/bin/* /bin
    9  ln -s /opt/conda/pkgs/*/lib/* /usr/lib
   10  ln -s /opt/conda/pkgs/*/bin/* /bin
   11  ln -s /opt/conda/pkgs/*/lib/* /usr/lib
   12  /opt/conda/bin/conda install -c conda-forge -y jupyterlab=1.2.3 #document the version of the program
   13  /opt/conda/bin/conda install -c conda-forge -y nodejs=10.13.0
   14  /opt/conda/bin/pip install bash_kernel
   15  /opt/conda/bin/pip install ipykernel
   16  /opt/conda/bin/python3 -m bash_kernel.install
   17  /opt/conda/bin/conda search htseq
   18  /opt/conda/bin/conda search-c bioconda htseq
   19  /opt/conda/bin/conda search -c bioconda htseq
   20  /opt/conda/bin/jupyter lab --no-browser --allow-root --ip=0.0.0.0 --NotebookApp.token='' --NotebookApp.password='' --notebook-dir='/scratch/reproducibility-tutorial/'
   21  #Control C gets you out of Jupyter and back to the terminal
   22  /opt/conda/bin/conda search -c bioconda snakemake
   23  /opt/conda/bin/conda install -c bioconda -c conda-forge -y snakemake=5.8.1
   24  ln -s /opt/conda/bin/* /bin
   25  ln -s /opt/conda/lib/* /usr/lib
   26  snakemake --version
   27  sudo apt-get update
   28  sudo apt-get install -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common
   29  curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
   30  sudo add-apt-repository  "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
 $(lsb_release -cs) \
 stable"
   31  sudo apt-get update
   32  sudo apt-get install -y docker-ce docker-ce-cli containerd.io
   33  docker run hello-world
   34  cd /scratch/reproducibility-tutorial/
   35  cd /scratch/reproducibility-tutorial# history >>README.md
   36  history
   37  #the command 'history' provides a list of command
   38  nano README
   39  nano README.md
   40  history >>README.md
