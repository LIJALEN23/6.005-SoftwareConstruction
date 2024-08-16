# 测试
- Test-first programming. Write tests before you write code. 测试优先的编程。在编写代码之前先编写测试。
- Systematic testing with partitioning and boundary values, to design a test suite that is correct, thorough, and small. 使用分区和边界值进行系统测试，以设计正确、彻底且小型的测试套件。
- Glass box testing and statement coverage for filling out a test suite. 用于填写测试套件的玻璃盒测试和声明覆盖范围。
- Unit-testing each module, in isolation as much as possible. 尽可能隔离地对每个模块进行单元测试。
- Automated regression testing to keep bugs from coming back. 自动回归测试可防止错误再次出现。
- Iterative development. Plan to redo some work. 迭代开发。计划重做一些工作。

## Validation验证
- Formal reasoning：自动化验证工具
- Code review：让其他人阅读代码
- Testing：精心选择输入来测试程序

## Software testing is hard软件测试的难点
- Exhaustive testing：不可能将所有的情况测试完
- Haphazard testing：
- Random or statistical testing：

## Test-first programming优先测试编程
- 术语(term)：
  - module模块：是软件系统的一部分，可以与系统的其余部分分开设计、实现、测试和推理。
  - specification规范：描述模块的行为。
  - implementation实现：实现一个模块的功能
  - test case测试用例：即测试用例
  - test suite测试套件：模块的一组测试用例

测试优先编程的最大好处是避免错误。不要等到开发结束时才进行测试，此时您有大量未经验证的代码。将测试留到最后只会使
调试时间更长、更痛苦，因为错误可能存在于代码中的任何地方。在开发代码时测试代码要愉快得多
- 流程：
  1. 写规范
  2. 写测试
  3. 实现

## Systematic testing系统测试
- 原则：
  - Correct正确的
  - Thorough彻底的
  - Small小的

## Choosing test cases by partitioning通过分区选择测试案例
- 即将测试分成小的子集来分别测试

## Automated unit testing with JUnit使用JUnit进行单元测试

## Documenting your testing strategy记录您的测试策略

## Black box and glass box testing黑盒和玻璃盒测试
- 黑盒测试：意味着仅从规范中选择测试用例，而不是从功能的实现中选择测试用例。这就是我们迄今为止在示例中所做的事情。我们划分并寻找abs 、 max和multiply的边界，而不查看这些函数的实际代码。事实上，按照测试优先的编程方法，我们甚至还没有编写这些函数的代码。
- 玻璃箱测试：意味着在了解功能实际实现方式的情况下选择测试用例。例如，如果实现根据输入选择不同的算法，那么您应该围绕选择不同算法的点进行分区。如果实现保留了一个记住先前输入答案的内部缓存，那么您应该测试重复的输入。

## Coverage覆盖范围
- 语句覆盖率：每个语句都由某个测试用例运行吗？
- 分支覆盖率：对于程序中的每个if或while语句，某个测试用例是否同时采用 true 和 false 方向？
- 路径覆盖：是否每个可能的分支组合（程序中的每条路径）都被某个测试用例采用

## Unit and integration testing单元和集成测试
- 单元测试：隔离测试单个模块。单独测试模块可以使调试变得更加容易。当模块的单元测试失败时，您可以更加确信错误是在该模块中找到的，而不是在程序中的任何地方。
- 集成测试：测试模块的组合，甚至整个程序

## Automated regression testing自动回归测试

## Iterative test-first programming迭代测试优先编程