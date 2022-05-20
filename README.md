# PyPi_structure
Package structure to build and deploy.

<b>step 1 : </b>fork reposetory. <br>
<b>step 2 : </b>Edit setup.cfg file.<br>
<b>step 3 : </b>Create accounts for the Test PyPI and PyPI repositories.<br>
<b>step 4 : </b>build using <br>
            (if windows) ```py -m build```<br>
            (if Unix/macOS) ```python3 -m build```
            
<br>Will generate  following files inside dist directory.<br>
                1) example-package-YOUR-USERNAME-HERE-0.0.1-py3-none-any.whl <br>
                2) example-package-YOUR-USERNAME-HERE-0.0.1.tar.gz    

<br><b>step 5 : </b>install twin using <br>
            (if windows) ```py -m pip install --upgrade twine``` <br>
            (if Unix/macOS) ```python3 -m pip install --upgrade twine```
            <br>

<b>step 6 : </b>deploy package using <br>
            (if windows) ``` py -m twine upload --repository testpypi dist/*``` <br>
            (if Unix/macOS) ``` python3 -m twine upload --repository testpypi dist/*```
            <br>
