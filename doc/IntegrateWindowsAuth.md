# Windows整合式驗證:
  
### 前導知識:

* **Windows相關帳戶(**重要!建議先搞懂**)**:
  * MS SQL資料庫主要連線帳戶種類:
  ![image](https://user-images.githubusercontent.com/14270012/88496615-55fd8480-cff0-11ea-9f9e-be033a8bc1d5.png)
  Once you know the name of the account running the SQL Server service, you must locate it in Active Directory. The account can be in a few possible locations depending on
  whether it is a local virtual account, a domain account, or a Managed Service account.
  
    [**Reference**:SQL Server domain authentication problems](https://help.deepsecurity.trendmicro.com/12_0/on-premise/kerberos-mssql.html)
  
  * [SQL Server-Configure Windows Service Accounts and Permissions](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/configure-windows-service-accounts-and-permissions?view=sql-server-ver15)
  * [Local System、Local Service與Network Service的不同](https://blog.darkthread.net/blog/local-system-local-service-network-service/)
  * [如何配置託管服務帳號(MSA)](https://www.twblogs.net/a/5b9708682b717750bda88976)
  * [How To Configure Managed Service Accounts Windows Server 2016](http://www.ntweekly.com/2018/02/07/configure-managed-service-accounts-windows-server-2016/)
  * [使用MSA(Managed Service Accounts)建置SQL服務](https://dotblogs.com.tw/jamesfu/2012/07/04/managedserviceaccounts)
  * [Windows安全性-存取控制概觀](https://docs.microsoft.com/zh-tw/windows/security/identity-protection/access-control/access-control)

* **SPN(Service Principal Names)**
  * [SPN-Microsoft官方文件](https://docs.microsoft.com/en-us/windows/win32/ad/service-principal-names)
  * [How to Use SetSPN to Set Active Directory Service Principal Names](https://petri.com/how-to-use-setspn-to-set-active-directory-service-principal-names-2)
  * [How to use SPNs when you configure Web applications that are hosted on Internet Information Services](https://support.microsoft.com/en-us/help/929650/how-to-use-spns-when-you-configure-web-applications-that-are-hosted-on)
  * [Register a Service Principal Name for Kerberos Connections](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/register-a-service-principal-name-for-kerberos-connections?view=sql-server-ver15)

* **Kerberos 與 NTLM 驗證**
  * [Windows驗證歷程觀察與Kerberos/NTLM判別](https://blog.darkthread.net/blog/check-auth-method-of-browser/)
  * [關於IIS整合式Windows驗證的冷知識](https://blog.darkthread.net/blog/ntlm-and-kerberos-on-iis/)
  
* **AD(Active Directory)**
  * [Server 2008 R2 Active Directory建置實務-網域與樹系信任概觀](http://epaper.gotop.com.tw/pdf/aca015200.pdf)


### 相關實例:
* [運作原理簡述](https://www.chainnews.com/zh-hant/articles/094369852800.htm)
* [部署內部網站並使用 Windows 驗證登入的標準作業流程](https://blog.miniasp.com/post/2014/01/12/Deployment-Intranet-Sites-using-Windows-Authentication-SOP)
* [介紹 IIS 7.5 的應用程式集區與新增的「虛擬帳戶」特性](https://blog.miniasp.com/post/2009/09/09/Introduce-IIS-75-Application-Pool-Identity-and-Virtual-Account)
* [Java使用windows驗證方式連接sqlserver2008數據庫-程式範例](https://www.itread01.com/content/1511947354.html)
* [Microsoft JDBC Driver for SQL Server](https://docs.microsoft.com/zh-tw/sql/connect/jdbc/working-with-a-connection?view=sql-server-ver15)

### TroubleShoot:
* [Troubleshooting Kerberos failures in Internet Explorer](https://support.microsoft.com/en-us/help/4551934/kerberos-failures-in-internet-explorer)
* [SQL Server domain authentication problems](https://help.deepsecurity.trendmicro.com/12_0/on-premise/kerberos-mssql.html)
* [無法使用Windows帳號登入防火牆內的SQL Serve](https://blog.darkthread.net/blog/ssms-sspi-firewall-issue/)
* [為什麼 Web 應用程式已經啟用Windows驗證，仍會提示要求輸入使用者名稱和密碼？](https://dotblogs.com.tw/terrychuang/2012/05/25/72388)
* [如何設定 Internet Explorer 自動登入使用 AD 認證的網站，或設定不要自動登入](https://support.microsoft.com/zh-tw/help/978218)


### 其他資料:

* [VMware-如何於虛擬主機建置時，以本機機器帳戶做為 SPN (服務主體名稱):Active Directory 身分識別來源設定](https://docs.vmware.com/tw/VMware-vSphere/5.5/com.vmware.vsphere.security.doc/GUID-4D24C6E8-63F5-4E35-862E-B59A03703254.html)
* [Add a vCenter Single Sign On (SSO) Active Directory (AD) Identity Source](https://www.vkernel.ro/blog/add-a-vcenter-single-sign-on-sso-active-directory-ad-identity-source)

 
