During testing, Swagger leaks are occasionally encountered. Common leaks are shown in the image:
(Specific image of Swagger leak)

Some leaks involve numerous interfaces, and it's practically impossible to manually test each one. Therefore, I wrote a Python script to automatically crawl all interfaces, configure the parameters, and send packets for access.

**The first version was only adapted for one version of Swagger. Significant differences exist between versions. Subsequent investigations covered many versions of Swagger, greatly enhancing the script's adaptability.**

Optimizations include:
- Adaptation to multiple versions of Swagger
- Addition of multiprocessing
- Enhanced robustness of the program
- Improved console display and log file generation

Single link format:
(Specific image of the single link format)
File format:
(Specific image of the file format)

Final result:
(Specific image of the final result)

# Swagger-hack 2.0

在测试中偶尔会碰到swagger泄露
常见的泄露如图：
![](https://github.com/jayus0821/swagger-hack/blob/main/images/image-20210201200842378.png)
有的泄露接口特别多，每一个都手动去试根本试不过来
于是用python写了个脚本自动爬取所有接口，配置好传参发包访问

**第一个版本仅适配了一个版本的swagger，不同版本见差距比较大，后续又调查了很多版本的swagger，将脚本的适配性增强了很多**

优化：
* 适配多个版本swagger
* 添加多进程
* 增强了程序的健壮性
* 优化了控制台显示，生成日志文件

单链接形式：
![](https://github.com/jayus0821/swagger-hack/blob/main/images/1.png)
文件形式：
![](https://github.com/jayus0821/swagger-hack/blob/main/images/2.png)

最终结果：
![](https://github.com/jayus0821/swagger-hack/blob/main/images/image-20210201201527999.png)


