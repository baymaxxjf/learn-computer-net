# learn-computer-net

添加静态路由方法
ROUTE [-f] [-p] [-4|-6] command [destination] [MASK netmask]  [gateway] [METRIC metric]  [IF interface]

  -f           清除所有网关项的路由表。如果与某个
  
               命令结合使用，在运行该命令前，
               
               应清除路由表。
               
  -p           与 ADD 命令结合使用时，将路由设置为
  
               在系统引导期间保持不变。默认情况下，重新启动系统时，
               
               不保存路由。忽略所有其他命令，
               
               这始终会影响相应的永久路由。Windows 95
               
               不支持此选项。
               
  -4           强制使用 IPv4。
  
  
  -6           强制使用 IPv6。
  

  command      其中之一:
  
                 PRINT     打印路由
                 
                 ADD       添加路由
                 
                 DELETE    删除路由
                 
                 CHANGE    修改现有路由
                 
                 
  destination  指定目的主机或者目的网段的网络地址。
  
  MASK         指定下一个参数为“网络掩码”值。
  
  netmask      指定此路由项的子网掩码值（目的主机或者目的网段的子网掩码）。
  
               如果未指定，其默认设置为 255.255.255.255。
               
  gateway      指定网关（下一跳）。
  
  interface    指定路由的接口号码。
  
  METRIC       指定跃点数，例如目标的成本。
  
  eg：route -p add 210.38.0.0/16 [默认网关]
