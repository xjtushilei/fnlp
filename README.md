# fnlp

复旦NLP的maven使用，并给出了一些例子


# 如何使用

### maven 引入

fnlp的maven仓库貌似除了问题，我们不能直接用maven了，所以采用了本地引入jar包的方式。


```
        <dependency>
            <groupId>org.fnlp</groupId>
            <artifactId>core</artifactId>
            <version>2.1</version>
            <scope>system</scope>
            <systemPath>${basedir}/libs/fnlp-core-2.1-SNAPSHOT.jar</systemPath>
        </dependency>
        <dependency>
            <groupId>org.fnlp</groupId>
            <artifactId>app</artifactId>
            <version>2.1</version>
            <scope>system</scope>
            <systemPath>${basedir}/libs/fnlp-app-2.1-SNAPSHOT.jar</systemPath>
        </dependency>
```

jar 包在我的项目根目录下的libs里面，该方法适用于任何其他项目里用到非官方库的方法。

### 模型文件引入

其实放哪里都行。不过最好还是放绝对路径吧，单独运行文件和打成war包使用会引起好多问题。


### 功能测试

demo 里有一些nlp的功能示例，比如分词，实体识别，关键词识别，时间识别等。


# 最后

弃疗吧。fnlp都没人维护这个垃圾代码了，之前感觉很好用。现在回头来看，在代码设计上距离工程化还是有许多的差距的。

