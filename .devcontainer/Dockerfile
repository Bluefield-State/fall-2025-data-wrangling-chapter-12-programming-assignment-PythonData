# Use a base image with Python
FROM continuumio/miniconda3

# Set the working directory
WORKDIR /workspace

# Install required packages
RUN conda install -y \
    pandas jupyter matplotlib lxml beautifulsoup4 html5lib openpyxl requests \
    sqlalchemy seaborn scipy statsmodels patsy scikit-learn pyarrow pytables numba ipython && \
    conda clean -afy

# Set the default command to run Jupyter Notebook
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--no-browser", "--allow-root"]