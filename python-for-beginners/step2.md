Once the installation is completed. We can start the container to give us an interactive Python shell using Jupyter Notebook. To start the Jupyter Notebook from the image use :

`docker run -i -t -p 8888:8888 continuumio/anaconda3 /bin/bash -c "/opt/conda/bin/conda install jupyter -y --quiet && mkdir /opt/notebooks && /opt/conda/bin/jupyter notebook --notebook-dir=/opt/notebooks --ip='*' --port=8888 --no-browser --alow-root"`{{execute}}

Once its successfully launched, you will see the output similar to 

    The Jupyter Notebook is running at: 
    http://127.0.0.1:8888/?token=6d967a0b65206dfa01437829d063c269ef9c5b654ec32025

You will need to copy the token for eg: **6d967a0b65206dfa01437829d063c269ef9c5b654ec32025** to use in the next step.
