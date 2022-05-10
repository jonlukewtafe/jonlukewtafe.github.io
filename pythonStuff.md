# Python Information

- ## PEP-8 Information
  
  The below links provide information about how to style your Python code into the PEP-8 style

  - [Official PEP-8 Style Guide for Python Code](https://www.python.org/dev/peps/pep-0008/)
  - [How to Write Beautiful Python Code With PEP-8](https://realpython.com/python-pep8/)
  - [Clean Code in Python](https://testdriven.io/blog/clean-code-python/)

- ## Guides and Other Useful Information
  - [A Guide to Python's Magic Methods](https://rszalski.github.io/magicmethods/)
  - []()
  - []()
  
- ## Keeping Track of Packages in Python Projects (AKA Freezing Requirements)
  - Freezing requirements allows for simple installation of packages upon a Python program/application being pulled from Git (or similar).
  - In order to freeze requirements, run: `pip freeze > requirements.txt` This will print a list of Python packages that are currently being used/installed as a part of the current project to the file `requirements.txt`.
  - Ensure that this is done prior to submission of any assessment work that uses packages as it makes it simple to install the required packages, requiring only a single command once the application is pulled from Git (or similar)
    - The command: `pip install -r requirements.txt`

{% include_relative footer.md %}
