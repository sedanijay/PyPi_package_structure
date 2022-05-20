# PyPi_structure
Package structure to build and deploy.

<b>step 1 : </b>fork reposetory. <br>
<b>step 2 : </b>Edit setup.cfg file.<br>
<b>step 3 : </b>Create accounts for the Test PyPI and PyPI repositories.<br>
<b>step 4 : </b>build using <br>
            ```(if windows) py -m build
               (if Unix/macOS) python3 -m build
            ```
<br>Will generate  following files inside dist directory.<br>            
                ```example-package-YOUR-USERNAME-HERE-0.0.1-py3-none-any.whl ```<br>
                ```example-package-YOUR-USERNAME-HERE-0.0.1.tar.gz```            

<b>step 5 : </b>install twin using 
            ```(if windows) py -m pip install --upgrade twine``` <br>
            ```(if Unix/macOS) python3 -m pip install --upgrade twine```
            <br>

<b>step 6 : </b>deploy package using 
            ``` (if windows) py -m twine upload --repository testpypi dist/*``` <br>
            ``` (if Unix/macOS) python3 -m twine upload --repository testpypi dist/*```
            <br>
