# 环境依赖说明

## 核心组件版本

| 技术组件       | 版本号       |
|---------------|-------------|
| Apache Spark  | 2.4.0       |
| Scala         | 2.11.12     |
| Java (JDK)    | 1.8         |
| Apache Hadoop | 2.7         |

## 兼容性说明

1. **Scala 版本要求**  
   - Spark 2.4.0 必须使用 **Scala 2.11.x** 系列版本
   - 不兼容 Scala 2.12+ 版本

2. **Java 版本要求**  
   - 仅支持 **Java 8（JDK 1.8）** 运行环境
   - 不支持 Java 9+ 及以上版本

3. **Hadoop 支持范围**  
   - 兼容 Hadoop 2.7.x 分支版本
   - 需配置 `HADOOP_CONF_DIR` 环境变量

4. **部署注意事项**  
   ```bash
   # 环境变量配置示例
   export SPARK_HOME=/opt/spark-2.4.0-bin-hadoop2.7
   export PATH=$PATH:$SPARK_HOME/bin
