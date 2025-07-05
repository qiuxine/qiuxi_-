<h2 id="LM9qV">打开适用于Linux的Windows子系统和虚拟机平台</h2>
![](https://cdn.nlark.com/yuque/0/2025/png/34845511/1740358564277-7af83c95-b78a-4012-8507-df8aa317efca.png)

<h2 id="RGvHQ">2.<font style="color:rgb(64, 64, 64);">以 管理员身份 打开 PowerShell，运行以下命令：</font></h2>
```plain
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

**<font style="color:rgb(64, 64, 64);">重启电脑</font>**<font style="color:rgb(64, 64, 64);"> 使更改生效。</font>



<h2 id="HpwiM">3.下载并安装wsl2内核更新</h2>
<font style="color:rgb(64, 64, 64);">访问微软官方下载页面：  
</font><font style="color:rgb(64, 64, 64);"></font><font style="color:rgb(64, 64, 64);"> </font>[WSL2 Linux 内核更新包](https://aka.ms/wsl2kernel)<font style="color:rgb(64, 64, 64);">  
</font><font style="color:rgb(64, 64, 64);">下载并运行安装程序。</font>



<h2 id="xu5gI">4.设置wsl2为默认版本</h2>
<font style="color:rgb(64, 64, 64);">重启后，在 PowerShell 中运行：</font>

```plain
wsl --set-default-version 2
```



<h2 id="MUhRC">5.安装Linux发行版</h2>
1. <font style="color:rgb(64, 64, 64);">打开</font><font style="color:rgb(64, 64, 64);"> </font>**<font style="color:rgb(64, 64, 64);">Microsoft Store</font>**<font style="color:rgb(64, 64, 64);">，搜索并选择 Linux 发行版（如 Ubuntu、Debian 等）。</font>
2. <font style="color:rgb(64, 64, 64);">点击“获取”并安装。</font>
3. <font style="color:rgb(64, 64, 64);">安装完成后，从开始菜单启动，按提示设置用户名和密码。</font>

<font style="color:rgb(64, 64, 64);"></font>

<h2 id="IPd48"><font style="color:rgb(64, 64, 64);">6.验证安装</font></h2>
<font style="color:rgb(64, 64, 64);">查看已安装的 WSL 发行版及其版本：</font>

```plain
wsl -l -v
```

<font style="color:rgb(64, 64, 64);">输出中应显示 </font>`<font style="color:rgb(64, 64, 64);">VERSION 2</font>`<font style="color:rgb(64, 64, 64);">，表示 WSL2 已启用</font>

