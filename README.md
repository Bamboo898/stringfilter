# Property Filter
此项目属于Property的工具类。主要作用是通过反射拿到对象中的值并对值进行转化处理，最终得到一个字符串。

## 安装
```
git clone https://github.com/Bamboo898/property-filter.git
cd property-filter
mvn clean install -Dmaven.test.skip=true
```
执行以上命令后可在项目中加入maven依赖，如下:
```
<dependency>
	<groupId>com.gs.utils</groupId> 
	<artifactId>property-filter</artifactId>
	<version>1.0</version>
</dependency>
```

## 用法
```
PropertyUtils.getProperty(user, "mobileNumber|mask:'3':'4'");
```
或者
```
PropertyUtils.getProperty(user, "status|dynDesc:'common.user.status'", applicationContext);
```
