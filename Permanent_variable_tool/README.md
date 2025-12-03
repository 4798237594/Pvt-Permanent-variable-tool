# Permanent Variable Tool
### 中文文档请往下查看
---
## `pvt.new(variable:str, value:Any=None) -> None`
Functionality

Creates/updates variable files in `./data/` directory 
### Usage Example 
```python
pvt.new("user_profile", {"name": "John", "age": 28})  # Serializes to string 
pvt.new("system_flag")   # Creates empty file 
```
---
## `pvt.read(variable:str) -> str`
### Critical Notes
- Always wrap in try-except:
```python 
try:
    config = pvt.read("app_config")
except FileNotFoundError:
    initialize_defaults()
```
---
## `pvt.delete(variable:str) -> None`
### Security Notice 
- Deletion is permanent. Recommended safety check:
```python 
if os.path.exists(pvt.data_dir + "/" + variable + ".var"):
    pvt.delete("temp_data") 
```
---
## `pvt.find (variable name: str) -> Bool`
### Use examples
```python
Bool = pvt.find(str)
print(Bool) # True / False
```
---
---

# 永久变量工具 (Permanent Variable Tool)
### Please check the English documents up.
---
## `pvt.new(变量名:str, 值:Any=None) -> None`
功能 
在`./data/`目录中创建/更新变量文件
### 使用示例 
```python
pvt.new("user_profile", {"name": "张三", "age": 28})  # 序列化为字符串 
pvt.new("system_flag")   # 创建空文件
```
--- 
## `pvt.read(变量名:str) -> str`
### 重要说明 
- 必须使用try-except包裹:
```python 
try:
    config = pvt.read("app_config")
except FileNotFoundError:
    initialize_defaults()
```
---
## `pvt.delete(变量名:str) -> None`
### 安全提示 
- 删除操作不可逆。建议进行安全检查:
```python 
if os.path.exists(pvt.data_dir + "/" + variable + ".var"):
    pvt.delete("temp_data")
```
---
## `pvt.find(变量名:str) -> Bool`
### 使用示例 
```python 
Bool = pvt.find(str)
print(Bool) # True / False
```