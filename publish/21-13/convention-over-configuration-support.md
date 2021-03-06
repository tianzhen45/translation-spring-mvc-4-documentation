# 21.13 "约定优于配置"的支持

对于许多项目来说，不打破已有的约定，对于配置等有可预测的默认值是非常适合的。现在，Spring MVC对 _约定优于配置_ 这个实践已经有了显式的支持。这意味着什么呢？意味着如果你为项目选择了一组命名上的约定/规范，你将能减少 _大量_ 的配置项，比如一些必要的处理器映射、视图解析器、`ModelAndView`实例的配置等。这能帮你快速地建立起项目原型，此外在某种程度上（通常是好的方面）维护了整个代码库的一致性should you choose to move forward with it into production.

具体来说，支持“约定优于配置”涉及到MVC的三个核心方面：模型、视图，和控制器。
