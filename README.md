front是前端vue项目文件，集成vue脚手架开发，前端项目端口号:8080

ylb是后端SpringBoot+Dubbo+zookeeper+MyBatis项目

整体是一个微服务互联网金融理财项目

微服务项目介绍

micr-api:普通maven项目，用于提供数据模型和基本service接口

micr-common:普通maven项目，用于提供公共的常量与工具

micr-parent:普通maven项目,所有项目的父项目

micr-dataservice:SpringBoot项目，为其余项目提供数据服务，生成mapper接口查询数据库

micr-task:SpringBoot项目，定时任务服务

micr-pay:SpringBoot项目向外提供web服务，支付功能服务    端口号:9000

micr-web:SpringBoot项目向外提供web服务，提供基本的接口服务  端口号:8000



注意:在micr-pay服务中，service实现类中，需要将url改为该服务进行内网穿透的地址
![image](https://github.com/Tianwailaiwu1/finance-project/assets/120568732/841f07ac-a957-4bfa-845c-8387ed80dc68)


