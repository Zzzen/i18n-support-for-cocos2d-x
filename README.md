## i18n-support-for-cocos2d-x
## 为cocos2d-x添加国际化支持

主要思路：
  - 将各种语言的翻译用json储存，放到Resources下面的i18n文件夹；
  - 运行时，根据所在地区选择对应的语言文件

目前具体实现：
  1. 在一个translation.txt内，储存key，英文，中文，以'#'作为分隔符；
  2. 用nodejs根据translation.txt生成对应的en.json, zh.json，以及i18n.h（存放Key）；
  3. 在运行时，读取json文件（参照i18n.cpp）；

## LICENSE: WTFPL
