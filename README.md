# XmlToWord

 ![jdk1.6+](https://img.shields.io/badge/jdk-1.6%2B-orange.svg) ![jdk1.8](https://img.shields.io/badge/jdk-1.8-orange.svg) 

XmlToWord基于[Apache FreeMarker](https://freemarker.apache.org)，遵从*模板 + 数据模型 = 输出*的理念，
通过极简API即可实现自定义模板Word的输出，可实现以下功能：

  * 基本文本的输出，文本占位符样式即输出文本样式。
  * 文本行、表格行单行或多行的遍历输出，并能够进行循环嵌套输出。
  * 提供数据处理的插件，通过添加处理器可定制任意输出值，例如：常见特定项的日期、数字等文本格式问题
  * 图片保留样式的输出。
  * 后期增加单元格的合并功能。


## 快速开始
Maven

```xml

```
```java
  
  HashMap<String, Object> data = new HashMap<>();
  ...准备数据
  data.put("zxsm",zxsmList);
  data.put("sbsm","kmood-导出-商标说明");
  
  DocumentProducer dp = new DocumentProducer("./ActualModelGeneratePath/");
  dp.Complie("./xmlModelPath/",true);
  dp.produce(data,"./wordExportPath/test.doc");
```
###实现效果

## 详细文档与示例


## 架构设计


## 建议和完善
参见[常见问题]()，欢迎在GitHub Issue中提问和交流。
