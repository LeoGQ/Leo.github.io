**交易账户实现多人下单 分仓系统 交易外接 多指令管理**
<br />**指令管家下载：https://raw.githubusercontent.com/LeoGQ/quant/main/CommandKeeper/%E6%8C%87%E4%BB%A4%E7%AE%A1%E5%AE%B6.zip**
<br />**或项目地址：https://github.com/LeoGQ/quant/tree/main/CommandKeeper/指令管家.zip**
<br />实现多个交易员或基金经理同时委托，并将委托指令发送到同一台电脑，再由这台电脑生成指令文件（指令保存为messages.csv），最后通过券商或期货商的交易软件文件交互功能实现下单。
![image](https://github.com/LeoGQ/quant/assets/46437678/c1382f28-6350-4a58-94ec-c795b38ed94d)

<br />说明：<br />
1、 将指令管家服务端在具有固定IP的电脑上运行，用来收集不同交易员和基金经理的指令，并同步给交易软件的文件交互实现下单。<br />
2、 指令管家服务端的设置：IP地址，设置为本机的内部监控地址如：0.0.0.0或者localhost，端口自定义即可。（如有防火墙限制需放开相关防火墙限制）<br />
3、 指令管家客户端，用于不同的交易员或基金经理下单，IP地址为服务端的公网IP地址，端口必须与服务端的一致。<br />
4、 生成的指令文件需要根据对应交易软件的文件交互要求做调整。<br />
