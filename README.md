# [Deployment] Migrate python package to another computer

1. Update pip in target computer

`curl https://bootstrap.pypa.io/get-pip.py | python`

2. Enter the command below

Mac:
`yum update python-pip`  

Ubuntu:
`apt-get update && apt-get upgrade python-pip`
  
3. Upgrade setuptools

`pip install --upgrade setuptools`

4. Make a list of package requirement 
 
`pip freeze > req.txt`
 
5. Copy req.txt to target computer, then run

`pip install -r req.txt`
