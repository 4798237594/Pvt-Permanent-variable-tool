Change log  更改日志
[1.0.0] - 2025-11-25 
Add  新增
- Initial release  初始发布 
- Realization of basic functions  实现基本功能 
---
[1.0.1] - 2025-11-27 
Add  新增
- Fixed the problem that `FileNotFoundError` would prompt twice.
- 修复了 `FileNotFoundError` 会提示两次的问题。
- Fixed the problem that you had to use `pvt.new ('')` to create a storage folder when you first installed it.
- 修复了首次安装时必须使用 `pvt.new("")` 来创建存储文件夹的问题。
- More special variables are supported, for example:
- 支持更多特殊变量，例如：
```python
True
False
None
Ellipsis
NotImplemented 
```
---
[1.0.2] - 2025-11-27 
Add  新增
- Add Chinese documents  新增中文文档 
  - Joke: I'm a Chinese, but I didn't add Chinese the first time.
  - 笑话：我一个中国人竟然不第一时间加中文。
---
[1.0.3] - 2025-11-27 
Add  新增
- Added `pvt.find()` function to check if a variable file exists
- 新增 `pvt.find()` 函数用于检查变量文件是否存在 
- Optimized documentation structure and added usage examples for the new function 
- 优化文档结构，新增函数使用示例 
- Updated security check recommendations to use the new `pvt.find()` function 
- 更新安全检查建议，推荐使用新的 `pvt.find()` 函数
 
Fixed  修复 
- Corrected directory path information in documentation (from `./data/` to `C:\pvt_data\`)
- 修正文档中的目录路径信息（从 `./data/` 改为 `C:\pvt_data\`）
- Improved error handling consistency across all functions
- 改进所有函数的错误处理一致性
---
[1.0.4] - 2025-12-4
Add 新增
- Added `pvt.list` to output all variables to a list.
- 新增 `pvt.list` 将所有的变量输出到列表。