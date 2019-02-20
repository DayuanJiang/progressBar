# A simple console progress bar for Python 3  
`progressBar` is a simple progress bar that can show in the text console.    
![demo](src/progressBarDemoGIF.gif)  
Like the GIF shows, this tool can display the following information.  
![explain](src/progressBarExplain.png)


## Install
```
pip install console-progress-bar
```

## Usage
It is super easy to use.
```python
from progressBar import ProcessBar

bar = ProcessBar(99)

for i in range(1, 100):
    time.sleep(0.1)
    bar.update()
```
Explaining:

```python
from progressBar import ProcessBar

# initial bar object with the total number of task.
# it will print the title of the process bar.
bar = ProcessBar(99)

for i in range(1, 100):
    time.sleep(0.1)
    # Update for each completed task.
    # the text inside the parenthesise is optional. 
    bar.update("file {}".format(i))
```