## DataTypes

__Fundamental Data Types__

int  
float  
bool  
str  
list  
tuple  
set  
dict  

__Classes -> custom types__

__Specialized Data Types__

None

## Python program to find pip version

```python
from importlib import metadata

print("Pip Version : ",metadata.version("pip"))
pip_metadata = metadata.metadata("pip")
print(list(pip_metadata))
print("Homepage: ",pip_metadata["Home-page"])
print("Python requirements",pip_metadata["Requires-Python"])
```