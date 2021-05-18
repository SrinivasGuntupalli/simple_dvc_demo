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
Step18: tox command -
```
```bash
tox
for rebuilding -
```
```bash
tox -r 
pytest command
```
```bash
pytest -v
```
```bash
setup commands -
```
```bash
pip install -e . 
```
```bash
build your own package commands-

python setup.py sdist bdist_wheel

```