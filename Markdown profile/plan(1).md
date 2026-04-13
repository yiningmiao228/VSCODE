# Python 编程内功(计划版)


**每日时间投入：** 2 小时（包含手写代码与概念阅读）。
**核心铁律：前 8 周必须纯手写，绝对禁止使用 Claude/Copilot 等代码补全工具。** 只有大脑感到痛苦，肌肉记忆才能形成。

---

## 🟢 第一阶段：语法直觉与控制流 (Week 1 - Week 3)
*目标：建立与计算机对话的基础语感，告别 R 语言思维。*

### Week 1: 基础语法与逻辑控制
* **Day 1: 环境起步与变量。** 安装 Python 与 VS Code。练习 `print()`，理解 `int`, `float`, `str` 类型。
* **Day 2: 运算符与布尔逻辑。** `+`, `-`, `*`, `/`, `//`, `%`。掌握 `and`, `or`, `not`。练习：摄氏度转华氏度脚本。
* **Day 3: 条件分支。** `if`, `elif`, `else`。注意 Python 灵魂的**缩进**。练习：根据成绩输出 A/B/C/D 等级。
* **Day 4: While 循环。** 理解 `break` 和 `continue`。防范死循环。练习：写一个“猜数字”小游戏。
* **Day 5: For 循环基础。** 结合 `range()`。练习：计算 1-100 内所有奇数的和。
* **Day 6-7: 综合控制流。** 练习：纯手写打印九九乘法表；写一个寻找 100 以内所有素数的脚本。

### Week 2: 数据容器与增删改查
* **Day 1: 列表 (List)。** 索引与切片。练习：提取列表中后一半的元素并倒序打印。
* **Day 2: 列表的高级操作。** `.append()`, `.insert()`, `.pop()`。练习：用列表模拟排队叫号系统。
* **Day 3: 字典 (Dict)。** Key-Value 结构。练习：创建一个包含个人信息的字典，并实现动态更新。
* **Day 4: 嵌套结构。** 列表套字典/字典套列表（JSON 基础）。练习：记录 3 个学生的 3 门课成绩，并计算总分。
* **Day 5: 元组 (Tuple) 与集合 (Set)。** 元组的不可变性，集合的交并集与 O(1) 去重。练习：找出两个列表的公共元素。
* **Day 6-7: 容器实战。** 任务：利用字典和 While 循环，手写一个简单的“控制台通讯录管理系统”。

### Week 3: 函数封装与模块化
* **Day 1: DRY 原则与基础函数。** `def` 关键字与 `return`。练习：把第一周的温度转换写成通用函数。
* **Day 2: 作用域 (Scope)。** 局部变量 vs 全局变量。理解为什么不该在函数内直接修改全局变量。
* **Day 3: 灵活的参数。** 默认参数与关键字参数。练习：编写一个计算复利的函数。
* **Day 4: *args 与 **kwargs。** 动态参数解包。练习：写一个能接收任意数量数值并求平均值的函数。
* **Day 5: 模块导入 (Import)。** 使用 `math` 和 `random` 库。练习：生成随机数并计算标准差。
* **Day 6-7: 基础文件读写。** `open()`, `.read()`, `.writelines()`。练习：读取一个英文 txt 文件，统计单词出现频率（不用任何第三方库）。

---

## 🟡 第二阶段：内存模型与面向对象 (Week 4 - Week 6)
*目标：这是 R 转 Python 最痛苦的一关，搞懂“引用机制”和“对象思维”。*

### Week 4: 内存里的“便利贴”
* **Day 1: 对象的本质。** 变量只是标签。使用 `id()` 函数，对比 `is` 和 `==` 的区别。
* **Day 2: 可变与不可变 (Mutable vs Immutable)。** 为什么修改 List 会影响另一个变量，而修改 String 不会。
* **Day 3: 浅拷贝与深拷贝。** 引入 `copy` 模块。练习：手画多层嵌套列表被 `deepcopy` 后的内存指向图。
* **Day 4: 参数传递的坑。** 为什么千万不要把 `[]` 作为函数的默认参数。写代码验证这个经典的 Bug。
* **Day 5: 列表推导式 (List Comprehension)。** Pythonic 的写法。练习：把多行的 for 循环改写为单行推导式。
* **Day 6-7: 生成器 (Generator)。** 引入 `yield`。练习：写一个按块（Chunk）读取 GB 级别大文件的生成器，理解它如何节省内存。

### Week 5: 面向对象编程 (OOP) 启蒙
* **Day 1: 类与对象。** `class` 与 `__init__`。搞懂 `self` 到底是什么。
* **Day 2: 属性与方法。** 练习：定义一个 `Student` 类，封装计算平均分的方法。
* **Day 3: 类的组合。** 把一个类的实例作为另一个类的属性。练习：写一个 `Course` 类，塞进 `Student` 的课表中。
* **Day 4: 继承 (Inheritance)。** 父类与子类，`super()` 的用法。
* **Day 5: 闭包 (Closure) 与装饰器 (Decorator)。** 函数作为一等公民。
* **Day 6-7: 装饰器实战。** 练习：手写一个 `@timer` 装饰器，用来自动打印任意函数执行的耗时。

### Week 6: 高级特性与魔术方法
* **Day 1: 魔术方法 (Dunder Methods)。** `__str__`, `__len__`。让你的对象像内置数据一样好用。
* **Day 2: 迭代协议。** `__iter__` 与 `__next__`。
* **Day 3: 上下文管理器。** `with` 语法背后的 `__enter__` 和 `__exit__`。练习：手写一个文件操作的上下文管理器。
* **Day 4: 异常处理。** `try`, `except`, `finally` 与自定义 Exception 类。
* **Day 5-7: 综合 OOP 实战。** 任务：不依赖 sklearn，纯手写一个包含 `fit`, `predict` 和可视化格式输出的 `LinearRegression` 类结构。

---

## 🟠 第三阶段：算法思维与科学计算 (Week 7 - Week 9)
*目标：连接统计学博士的数学天赋，用算法结构大幅提升代码运行效率。*

### Week 7: 数据结构与算法 (LeetCode 基础)
* **Day 1: 时间/空间复杂度。** 理解 Big O Notation。
* **Day 2: 哈希表的威力。** LeetCode #1 两数之和。体会 O(1) 查找的恐怖速度。
* **Day 3: 双指针技术。** LeetCode #11 盛最多水的容器。优化内存占用。
* **Day 4: 栈与队列。** LeetCode #20 有效的括号。
* **Day 5: 树结构基础。** 递归思想与基线条件。
* **Day 6-7: 树的遍历。** LeetCode #104 最大深度, #226 翻转二叉树。为后续的决策树算法打基础。

### Week 8: 科学计算核心库 (回血周)
* **Day 1: NumPy 内存模型。** Ndarray 的连续内存块概念，对比原生 List。
* **Day 2: 广播机制 (Broadcasting)。** 彻底告别对数据的双层 `for` 循环。
* **Day 3: 高级索引。** NumPy 的切片与布尔索引。
* **Day 4: Pandas 基础。** DataFrame 就像数据库的表。
* **Day 5: 向量化操作。** `apply`, `groupby`, `merge`。
* **Day 6-7: 数据科学实战。** 任务：在 Jupyter Notebook 中，使用 Pandas 处理十万级真实开放数据集（处理缺失值、聚合统计），完全禁用 Python 原生循环。

### Week 9: 代码工程化与版本控制
* **Day 1: Git 基础操作。** `git init`, `add`, `commit`, `status`。
* **Day 2: 分支管理与冲突解决。** `branch`, `checkout`, `merge`，理解科研代码试错的正确姿势。
* **Day 3: GitHub 协作。** 推送本地代码，编写 Markdown 格式的 `README.md`。
* **Day 4: 虚拟环境。** 掌握 `conda` 或 `venv`，隔离不同项目的依赖包。`requirements.txt` 导出。
* **Day 5: 自动化与脚本化。** 使用 `os` 和 `pathlib` 批量重命名文件、处理杂乱的科研数据文件夹。
* **Day 6-7: 工程规范。** 学习 PEP 8 规范，使用 `flake8` 或 `black` 格式化你的代码。

---

## 🔴 第四阶段：深度学习架构与 AI 结对 (Week 10 - Week 16)
*目标：驾驭 PyTorch，掌握大模型生态，并最终利用 Claude Code 提升生产力。*

### Week 10: PyTorch 张量与动态图
* **Day 1: Tensor 基础。** Shape, View, Reshape, Squeeze。
* **Day 2: GPU 加速。** `.to('cuda')`，理解显存搬运过程。
* **Day 3: 自动微分机制 (Autograd)。** `requires_grad=True` 与 `.backward()` 的链式法则推导。
* **Day 4: 手写梯度下降。** 禁用 `torch.optim`，用张量操作纯手工更新权重参数。
* **Day 5: 面向对象的网络 `nn.Module`。** `__init__` 定义层，`forward` 定义计算流。
* **Day 6-7: 自定义数据管道。** 继承 `Dataset` 重写 `__getitem__`，结合 `DataLoader` 实现批处理 (Batching)。

### Week 11: 现代 AI 生态 (Hugging Face)
* **Day 1: Transformers 架构入门。** `Tokenizer` 与 `Model` 分离的逻辑。
* **Day 2: Pipeline 调用。** 用现成模型完成分类或抽取任务。
* **Day 3: Datasets 库原理。** 内存映射 (Memory-mapped) 读取海量数据。
* **Day 4: 模型内部探查。** 获取并分析语言模型输出的隐层状态 (Hidden States) 的高维统计特征。
* **Day 5-7: 深度微调实战。** 使用 PyTorch 结合开源权重，针对一个小型分类数据集跑通一次完整的微调训练闭环。

### Week 12: 大数据生态体系 (拓展储备)
* **Day 1: Parquet 格式与 PyArrow。** 告别低效的 CSV。
* **Day 2: 分布式计算初探。** Dask 基础，将 Pandas DataFrame 转为惰性计算。
* **Day 3: 并发计算。** `multiprocessing` 多进程，突破 GIL 锁运行 MCMC 统计模拟。
* **Day 4: 网络 IO 并发。** `asyncio` 异步抓取公开 API 数据。
* **Day 5-7: 性能调优分析。** 掌握 `cProfile` 和 `memory_profiler` 找出代码瓶颈。

### Week 13-16: 🎓 AI 协同与最终项目开发 (解禁 Claude Code)
> **阶段策略：** 此时你已具备极高的“代码鉴赏力”，可以直接指挥大模型替你写出高质量、符合架构规范的代码。

* **Week 13: 提示词工程与重构。** 练习让 Claude Code 根据你制定的接口（UML/伪代码）填写具体逻辑；让 AI 为你的科研旧脚本添加日志记录和完善的 `try-except` 错误处理。
* **Week 14: 测试驱动开发 (TDD)。** 学习 `pytest` 库。只手写最核心的统计函数计算逻辑，让 Claude 生成涵盖所有边界条件（极值、空值、类型错误）的单元测试断言。
* **Week 15-16: 结业项目开发（人机结对）。**
  * **选定课题：** 例如构建一个自动化流程，每天抓取 ArXiv 最新医学统计论文，利用大模型提取摘要，再用你的统计模型计算趋势，最后生成 Web 报告。
  * **分工协作：**
    * **你（大脑）：** 架构设计、数据结构选型、统计公式校对、系统 Debug。
    * **Claude Code（双手）：** 正则表达式清洗文本、API 调用封装、Matplotlib 美化制图、HTML 模板渲染。
  * **成果输出：** 一个结构完善、附带完整测试用例、推送到 GitHub 并带有一流 README 文档的顶级工程项目。