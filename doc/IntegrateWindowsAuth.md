# Windows整合式驗證:
  
### 前導知識:

* Windows相關帳戶:
  * [Configure Windows Service Accounts and Permissions](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/configure-windows-service-accounts-and-permissions?view=sql-server-ver15)
  * [介紹 IIS 7.5 的應用程式集區與新增的「虛擬帳戶」特性](https://blog.miniasp.com/post/2009/09/09/Introduce-IIS-75-Application-Pool-Identity-and-Virtual-Account)

* [Windows存取控制概觀(**重要!建議先搞懂**)](https://docs.microsoft.com/zh-tw/windows/security/identity-protection/access-control/access-control)

* [SQL Server-Configure Windows Service Accounts and Permissions](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/configure-windows-service-accounts-and-permissions?view=sql-server-ver15)
* SPN(Service Principal Names)
  * [SPN-Microsoft官方文件](https://docs.microsoft.com/en-us/windows/win32/ad/service-principal-names)
  * [How to Use SetSPN to Set Active Directory Service Principal Names](https://petri.com/how-to-use-setspn-to-set-active-directory-service-principal-names-2)
  * [How to use SPNs when you configure Web applications that are hosted on Internet Information Services](https://support.microsoft.com/en-us/help/929650/how-to-use-spns-when-you-configure-web-applications-that-are-hosted-on)
  * [Register a Service Principal Name for Kerberos Connections](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/register-a-service-principal-name-for-kerberos-connections?view=sql-server-ver15)

* Kerberos 與 NTLM 驗證

* AD(Active Directory)
 * [Server 2008 R2 Active Directory建置實務-網域與樹系信任概觀](http://epaper.gotop.com.tw/pdf/aca015200.pdf)



### 相關實例:
* [運作原理簡述](https://www.chainnews.com/zh-hant/articles/094369852800.htm)
* [部署內部網站並使用 Windows 驗證登入的標準作業流程](https://blog.miniasp.com/post/2014/01/12/Deployment-Intranet-Sites-using-Windows-Authentication-SOP)
* 

### TroubleShoot:
* [Troubleshooting Kerberos failures in Internet Explorer](https://support.microsoft.com/en-us/help/4551934/kerberos-failures-in-internet-explorer)
* [SQL Server domain authentication problems](https://help.deepsecurity.trendmicro.com/12_0/on-premise/kerberos-mssql.html)
* [無法使用Windows帳號登入防火牆內的SQL Serve](https://blog.darkthread.net/blog/ssms-sspi-firewall-issue/)


### 其他資料:
* [關於IIS整合式Windows驗證的冷知識](https://blog.darkthread.net/blog/ntlm-and-kerberos-on-iis/)
* [VMware-如何於虛擬主機建置時，以本機機器帳戶做為 SPN (服務主體名稱):Active Directory 身分識別來源設定](https://docs.vmware.com/tw/VMware-vSphere/5.5/com.vmware.vsphere.security.doc/GUID-4D24C6E8-63F5-4E35-862E-B59A03703254.html)
* [Add a vCenter Single Sign On (SSO) Active Directory (AD) Identity Source](https://www.vkernel.ro/blog/add-a-vcenter-single-sign-on-sso-active-directory-ad-identity-source)

 
