To create environment:

```
conda env create -f environment.yaml
conda activate ocp-tool
```

To use it for modifications based on FESOM meshes, please install pyfesom2 from the repository. Unfortunately, the latest conda package may not be updated to the changes needed to run OCP-Tool.

```
git clone https://github.com/FESOM/pyfesom2.git
conda env update --name ocp-tool --file ./pyfesom2/ci/requirements-py37.yml
cd pyfesom2
pip install -e
```

To run your conda environment as a kernel on jupyter notebook
```
conda install -c anaconda ipykernel
python -m ipykernel install --user --name=ocp-tool
```
