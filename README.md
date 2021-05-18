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
Step: touch train_and_evaluate.py
write the code
```
```bash
write code in dvc.yaml file for rain_and_evaluate and save the file and run the dvc file
Step: dvc repro






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