# problem  description
  As we all know,Python program usually depends on different repos,so we usually need to install the repos like
```python
    pip install ultralytics
```
but we will usually meet a error saying that we don't have the  authority to install a repo,which is designed to protect the inner  environment

# solution
we have to creat a virtual enviroment

    python3 -m venv venv
This will creat a directory named "venv",and then you need to source the virtual environment by 

    source venv/bin/activate

then you can see "(venv)" in front of your command line,that means you have sourced the virtual environment  successfully.
After that can you install the repos needed
if you wang quit the virtual environment,you can just

    deactivate
Besides,if you want save all the repos' versions,you can save them by creating a requirements.txt

    pip freeze > requirements.txt
this will create a requirements.txt which contains all the versions of the repos
next time if you want set up your repos,just

    pip -r install requirements.txt
