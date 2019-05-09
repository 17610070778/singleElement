# 作者：王亚奇 联系方式qq：1160782779
###这是一个用来改变编码方式的工具，大量使用lambda和函数式，使代码分块编写，便于开发人员阅读；可以用来提高代码的可阅读型，可维护性；
##工具开发的灵感来源：公司多人协同开发，代码不规范，相互维护代码简直就是灾难；作者使用过spring WebFlux开发过项目，特别喜欢里面的Flux与Mono流式操作编程，又因为java8有了Stream操作集合，在不使用WebFlux模块的情况下，操作单个元素的却没有，于是借鉴WebFlux的Mono自己开发了一套工具，目前工具API继续扩展中；

#API说明：
|--from(Supplier) 使用生成器来创建SingleElement
|--map(Function)  使用映射来转换元素
|--monitor(Consumer)  使用消费者来监控元素   