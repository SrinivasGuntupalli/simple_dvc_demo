```bash
Step 1: Create environment

conda create -n wineq python=3.7 -y
```
```bash
Step2: Activate environment

conda activate <your_env_name>
```
```bash
Step3: Create a requirement file

touch requirements.txt
```
```bash
Step4: runa requirement file

pip install -r requirements.txt
```
```bash
step5: create a template.py file

touch template.py
```
```bash
Step6: run the template.py file

python template.py
```
```bash
Step7: create a folder

mkdir data_given
```
```bash
Step8: download the data from gdrive and put it in data_given folder

https://drive.google.com/drive/folders/18zqQiCJVgF7uzXgfbIJ-04zgz1ItNfF5?usp=sharing

```
```bash
Step9: git init
```
```bash
Step10: dvc init 
```
```bash
Step11: dvc add data_given/winequality.csv
```
```bash
Step12: git add .
```
```bash
Step13: git commit -m "first commit"
```
```bash
#oneliner updates for readme

Step14: git add . && git commit -m "update Readme.md"
```
```bash
Step15: git remote add origin https://github.com/SrinivasGuntupalli/simple_dvc_demo.git
```
```bash
Step16: git branch -M main
```
```bash
Step17: git push origin main
```
```bash
update params.yaml file
Step: git add . && git commit -m "params added"
git push origin main
```
```bash
step: touch src/get_data.py
write code to bring data
```

```bash
Step: git add . && git commit -m "add get_data"
git push origin main
```
```bash
Step: touch src/load_data.py
write code 
```
```bash
Step: git add . && git commit -m "add get_data"
git push origin main
```
```bash
Step: python src/load_data.py
```
```bash
write code in dvc.yaml file for load_data and save the file and run the dvc file
Step: dvc repro
```
```bash
Step: git add . && git commit -m "stage 1 complete"
git push origin main
```
```bash
spliting file to split the data
Step: touch src/split_data.py
```
```bash
write code in dvc.yaml file for split_data and save the file and run the dvc file
Step: dvc repro
```
```bash
Step: git add . && git commit -m "stage 1 complete"
git push origin main
```
```bash
Step: touch src/train_and_evaluate.py
write the code
```
```bash
write code in dvc.yaml file for rain_and_evaluate and save the file and run the dvc file
Step: dvc repro
```
```bash
step: mkdir report
touch report/params.json
touch report/scores.json
```
```bash
Step: python src/train_and_evaluate.py
now model store the param values and metric scores in reports/param and scores file.
```
```bash
Step: dvc repro
dvc metrics show
dvc metrics diff
```
```bash
Step: git add . && git commit -m "Tracker Added"
git push origin main
```

```bash
Step: goto Params file and change the param values at estimators: section and save it and run the model
$ dvc repro
now check the scores and params json files
$ dvc metrics show
$ dvc metrics diff
```
```bash
creating the virtual test environments using [tox], it will help us to test our models in virtual environments with higher or lower versions Python versions.

step: touch tox.ini
write the code here
```
```bash
step: mkdir tests
touch tests/conftest.py touch tests/test_config.py
touch tests/__init__.py
```

```bash
Step:touch setup.py
write code here
```

```bash
Step: tox
this will create the test environment
```
```bash
Step: pytest -v
pip install -e .

pip freeze
this will tell you waht are all packages are installed in your current working directory.


```bash
tox command -
$ tox
```

```bash
tox for rebuilding -
$ tox -r
```
```bash
pytest command
$ pytest -v
```

```bash
setup commands -
pip install -e . 
```

```bash
build your own package commands-
$ python setup.py sdist bdist_wheel

```
```bash
Step: git add . && git commit -m "Set up is done"
git push origin main
```

```bash
you can install Jupyter notebook if you want
$ pip install jupyterlab
after installing it will display one link and it may look like this pyzmq-22.0.3
click on it, and $ prompt will come

$ jupyter-lab notebooks/
```

```bash
mkdir -p prediction_service/model
mkdir webapp
touch app.py
touch prediction_service/__init__.py
touch prediction_service/prediction.py
mkdir -p webapp/static/css
mkdir -p webapp/static/script
touch webapp/static/css/main.css
touch webapp/static/sctipt/index.js
mkdir webapp/templates
touch webapp/templates/index.html
touch webapp/templates/404.html
touch webapp/templates/base.html

add ll the codes in these files
```

```bash
Step: git add . && git commit -m "Added web stcture"
git push origin main
```

```bash
now build the FLASK api, for that we need to write a code in app.py file
```

```bash
now we need to implement the workflow which is call CI/CD
$ mkdir -p .github/workflow
$ touch .github/workflow/ci-cd.yaml

write the ci-cd code here
```
```bash
Step: git add . && git commit -m "Github action workflow added"
git push origin main
```
```bash
entrypoint for app
$ touch Procfile
specify the server name
```

```bash
Step: git add . && git commit -m "workflow updated"
git push origin main
```











