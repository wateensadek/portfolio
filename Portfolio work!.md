```python
print("Wateen Sadek, Dalhousie University")
```

    Wateen Sadek, Dalhousie University



```python
from IPython.display import HTML

styled_output = """<div style="font-family: Arial; font-weight: bold; font-size: 20px; color: blue;">
Wateen Sadek, Dalhousie University
</div>"""
HTML(styled_output)
```




<div style="font-family: Arial; font-weight: bold; font-size: 20px; color: blue;">
Wateen Sadek, Dalhousie University
</div>



You can use the following code to create a simple logo using the `matplotlib` library:


```python
import matplotlib.pyplot as plt

def create_logo(name):
    plt.figure(figsize=(6, 3))
    plt.text(0.5, 0.5, name, fontsize=40, ha='center', va='center', fontweight='bold', color='blue')
    plt.axis('off')
    plt.show()

create_logo("Wateen Sadek")
```




    
![png](Portfolio%20_files/Portfolio%20_3_0.png)
    


