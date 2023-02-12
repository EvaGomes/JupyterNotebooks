# Dockerized instance of JupyterLab v3.5.1, with IPython and IHaskell kernels

#############################################################################
# INSTRUCTIONS:
#############################################################################
# Pre-requisites: Having installed Docker in your system.
# 1. Open a command-line at the location you'll want to save your notebooks.
# 2. Build the Docker image using command:
#    > docker build -t jupyterlab-di .
# 3. Run a Docker container using command ...
#    ... on Windows OSs:
#    > docker run --rm -it -p 8888:8888 -v %cd%:/home/jovyan/src --name jupyterlab-dc jupyterlab-di
#    ... on Linux OSs:
#    > docker run --rm -it -p 8888:8888 -v $PWD:/home/jovyan/src --name jupyterlab-dc jupyterlab-di
# 4. Check the command output for a URL like `http://localhost:8888/lab?token=......`
# 5. Open it in a browser (Chrome, Firefox, ...)
#############################################################################

FROM gibiansky/ihaskell
EXPOSE 8888
VOLUME /home/jovyan/src
CMD jupyter-lab --ip=0.0.0.0
