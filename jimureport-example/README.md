# jimureport-example

积木报表集成示例代码。

```
采用mysql5.7数据库
```




使用步骤
-----------------------------------

-  第一步：执行初始化脚步（自动创建数据库jimureport）

           db/jimureport.mysql5.7.create.sql
           
-  第三步： 启动项目（右键运行）

           org.jeecg.modules.JimuReportApplication
           
-  第四步： 访问项目

      报表工作台： http://localhost:8085/jmreport/list
      
      仪表盘工作台： http://localhost:8085/drag/list
           




Docker镜像制作
-----------------------------------

-  第一步：下载项目

         git clone https://gitee.com/jeecg/JimuReport.git

-  第二步：进入项目 jimureport-example 根目录

         cd JimuReport/jimureport-example
	
-  第三步：maven执行package

         mvn clean package
		 
-  第四步：执行命令，生成镜像

>如果使用的是Mac M系列芯片，需要修改docker-compose.yml文件的第一行为：```FROM arm64v8/mysql:8```

         docker-compose up -d
		 
-  第五步：访问报表

      报表工作台： http://localhost:8085/jmreport/list
      
      仪表盘工作台： http://localhost:8085/drag/list
