> # <center>Corporate Portal </center>
![](https://bcp.mawarid.com.sa/UI/assets/images/mawarid-logo-2.png)
>## ***Login***

![](./BCP%20imgs/login%20.png)

  - username and password  call check user api .
  - if user exits call  SendOTP api.
- get otp  from 
[ **OTPLogLink**](https://bcp.mawarid.com.sa/logs/SMSLogger20231215.txt) →  ***`"Change corrent date and year in Url:"`*** 
 - enter OTP it will call validate OTP api then  go to home page.  
> ### **Application  Login Link & Credentials:**


[**CorporatePortal**](https://bcp.mawarid.com.sa/UI/#/CorporatePortal/home)  

[ **CorporateAdministration**](https://bcp.mawarid.com.sa/UI/#/Administration/dashboard) 

[ **CorporatePlatform**](https://bcp.mawarid.com.sa/UI/#/) 



  - ### *Register Mobile Number:* ###
    
      ![](./BCP%20imgs/Register%20mobile%20number.png)

  - ### *Update password Number:* ###
    
      ![](./BCP%20imgs/Update%20mobile%20number.png)

  - ### *Forgot Password:* ###
    
      ![](./BCP%20imgs/Forgot%20password.png)


# ***TopNav*** :

 - Call GetAllAccount get customer and prjoct then automatically bind  default Customer and project 
 - User can change cutomer and project 
 - Store in customer and project data in local storage 
than only work all page based on current Customer and project 
-open in home page
 
>## ***Menu:***
>  
 ![](./BCP%20imgs/menu.png)
   - Dash Board
   - Create Request
   - Iqama Expiry
   - Requests
   - Reports 
   - Time Sheet
   - Security
   - Admin Reports
   
># ***Dash Board***
  -  get list from crm/getrequests params: project id and 
  customer Details. 
  - data will get it from local stroge list of data.

# ***ApI:-***
   https://bcp.mawarid.com.sa/api/v2/crm/GetDashBoard
 
  ![](./BCP%20imgs/dash%20board.png)
      
># ***Customer Contract Count:***
  - Get list from crm /  Params: PageNo and page size in get local storage
  - data will get it from local storage
  - 
# ***API:-***

  ![](./BCP%20imgs/CustomerContractCount.png)

# ***Details:-***
  - details in Attachments button will show based on   condition 
  - if click details btn details will show in popup  
# ***API:-***

# ***General Notes:-***
  - createing notes in we get below fields Title,notes,file.

# ***API:-***         

># ***Contract New Labours:-***
  - Get list from crm /  Params: entity or RemoteEntity  in get local storage data.
  - data will get it from local storage.
  - 
# ***API:-***
   https://bcp.mawarid.com.sa/api/v2/crm/GetLaborListPaging?ProjectID
   ![](./BCP%20imgs/new%20labour%20contract.png)

# ***Details:-***
  - If click details list data  will show in popup in no data found. 


# ***General Notes:-***

># ***Create Request***
  -  Get list from crm /  Params: request type and  ticket gruop base in get local storage in total data.
  - data will get it request TypeEn base in data.
# ***API:-***

   https://bcp.mawarid.com.sa/api/v1/ticketmaster/group?RequesterTypeId
    

 ![](./BCP%20imgs/Create%20Request%202.png)
    
# ***Details:-***
  - if create request type in return request process and admin Request data details in this page. 
   

>#  ***Return Request Process:-***
  - Get crm / params get return reason get local storage in  customer-name base in get leave request ,final exit request , retrun request get local storage in get data .
  - 
# ***API:-***
    https://bcp.mawarid.com.sa/api/v2/crm/GetReturnReason?customer-name

![](./BCP%20imgs/Return%20Request%20Process.png) 

> # ***فشل في إجتياز الاختبارات المهنية***
> 
  - Get crm in Request / Params get documenttype and show attachment base get local storage in menu or EntityRecId base get data .

# ***API:-***
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/1.png)

# ***Details:-***
  - File attachment types Evidence Attachment , Clearance Attachment and EndOfContractAttachment in file attachment.
  - Employee Id based in get data .
  - 
  - __Notes__ search item in customer name or searchterm base get data in notes type.
  - 
# ***API:-*** 
  (https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm=&customer-name) 



># ***طلب إستقالة العامل وخروج نهائى***
  - Get crm in Request / Params get documenttype and show attachment base get local storage in menu or EntityRecId base get data .

# ***API:-***
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/2.png)

# ***Details:-***
  - File attachment types Evidence Attachment , Clearance Attachment and EndOfContractAttachment in file attachment.
  - Employee Id based in get data .
  - __Notes__ search item in customer name or searchterm base get data in notes type.
 
# ***API:-** 
  https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm=&customer-name

# ***إجازة مرضية مرتجع / خروج وعودة***

 - Get crm in Request / Params get documenttype and show attachment base get local storage in menu or EntityRecId base get data .

# ***API:-***
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/3.png)

# ***Details:-***
  - File attachment types Evidence Attachment , Clearance Attachment and EndOfContractAttachment in file attachment.
  - Employee Id based in get data .
  - __Notes__ search item in customer name or searchterm base get data in notes type.
  - Add time and date in add this data in Leave Start Date , Last Working day ,Required Days and Leave End Date in field in this request.
  
# ***API:-*** 
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId


# ***إجازة داخلية / خارجية***

  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/4.png)

# ***Details:-***
  - File attachment types Evidence Attachment , Clearance Attachment and EndOfContractAttachment in file attachment.
  - Employee Id based in get data .
  - __Notes__ search item in customer name or searchterm base get data in notes type.
  - Add time and date in add this data in Leave Start Date , Last Working day ,Required Days and Leave End Date in field in this request.
  
## ***API:-*** 
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId 


# ***الإعتداء على العامل / سوء التعامل مع العامل***

  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/5.png)

# ***Details:-***
  - File attachment types Evidence Attachment , Clearance Attachment and EndOfContractAttachment in file attachment.
  - Employee Id based in get data 
  - __Notes__ search item in customer name or searchterm base get data in notes type.
  
# ***API:-*** 
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId 


># ***طلب تأشيرة خروج و عودة*** 

  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/6.png)

# ***Details:-***
  - File attachment types Evidence Attachment , Clearance Attachment and EndOfContractAttachment in file attachment.
  - Employee Id based in get data .
  

  - Add time and date in add this data in Leave Start Date , Last Working day ,Required Days and Leave End Date in field in this request.
  -  __Remarks__ search item in customer name or searchterm base get data in notes type.
  
- ***API:-*** https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm=&customer-name

># ***طلب أجازة طارئة***
  https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId
    
  ![](./BCP%20imgs/7.png)

# ***Details:-***
  - File attachment types evidence attachment , clearance attachment and end Of contract attachment in file attachment.
  - Employee Id based in get data .
  

  - Add time and date in add this data in Leave Start Date , Last Working day ,Required Days and Leave End Date in field in this request.
  -  __Remarks__ search item in customer name or searchterm base get data in notes type.
  
# ***API:-*** 
https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm=&customer-name

># ***Admin Request***
- Admin request in get local storage get sub group or customer name Id put get admin request in data.
# ***API:-***
   https://bcp.mawarid.com.sa/api/v1/ticketmaster/subgroup/single/44?customer-name

   ![](./BCP%20imgs/1.1.png)

#  ***Renew Contract***
- get list from crm / get requests Params: activation recordor or customer name. 
- data will get it from local stroge 
# ***API:-***
https://bcp.mawarid.com.sa/api/v1/entitytype/form/activationrecord/63?customer-name

![](./BCP%20imgs/1.2.png)

# ***Notes***
- Renew contract get data in Customer name based get data in local storage in data.
-  __Notes__ search item in customer name or searchterm base get data in notes type.
# ***API*** 
   https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm
- Renew contract in renew employee or customer details and period and other details.

# ***Admin Request***
- Admin request get list from crm / get requests Params: activationrecordor or customer name. 
- data will get it from local stroge 
# ***API:-***
   https://bcp.mawarid.com.sa/api/v1/security/documenttype/showattachement?MenuOrEntityRecId

 ![](./BCP%20imgs/1.3.png)
# ***Notes:-***
-  __Notes__ search item in customer name or searchterm base get data in notes type.
  ## ***API:-*** 
  https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm
- Admin request in renew employee id or customer id details and request type language and other details.
  
# ***Letter Request***
 - letter  request in  get list form crm / get request params : letter type or customer type getdata in local storage.
 - data will get in form in letter request type customer id base in get it from local storage .
## ***API:-***
    https://bcp.mawarid.com.sa/api/v2/crm/GetLetterTypes?customer-name
![](./BCP%20imgs/1.4.png)

# Notes:-
  -  __Notes__ search item in customer name or searchterm base get data in notes type.
## ***API:-*** 
   https://bcp.mawarid.com.sa/api/v1/entitytype/cannedresponsebyshortcode?searchterm

># ***Iqama Expiry***
 - Iqama Expiry get in EntityTypeRecId based get it local storage in get data.
 - 
# ***API:-*** 
https://bcp.mawarid.com.sa/api/v1/entitytype/dynamic/get/?entityTypeRecId

![](./BCP%20imgs/Iqama%20Expiry.png)

# ***Notes***:-
  - Iqama exoiry get entityTypeRecId based in EmployeeID , CustomerId , ProjectID	,Name	, Iqama ,Subject	,IqamaExpiryDate , Description , IqamaPeriod	, Issued Date  ,RenewalStatus	and  Renewal Count.

# ***Workflow Details:-*** 
- NewRequest `01 - New` ➠ CustomerApproval `02 - InProgress` ➠SupervisorApproval `03 - InProgress` ➠ IqamaRenewal `04 - InProgress `➠ Completed `05 - Closed`
   - API:-
      https://bcp.mawarid.com.sa/api/v1/entitytype/batchqueue/byactionsstatus?actionStatus

> # ***Requests***

 ># ***Admin Requests***
   - get list from crm / GetRequests Params: ProjectID .
   -  data will get it from local stroge

# ***API:-*** 
  https://bcp.mawarid.com.sa/api/v2/crm/GetRequests?ProjectID

![](./BCP%20imgs/Admin%20Request.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  

# ***API*** 
   api/v2/crm/GetRequestByID?RequestID=e42c483f-529e-ee11-be37-0022489a5861

# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .


># ***Leave & Termination***
   - get list from crm / GetReturnRequestByProject Params: ProjectID .
   -  data will get it from local stroge

# ***API:-*** 
https://bcp.mawarid.com.sa/api/v2/crm/GetReturnRequestByProject?ProjectID

![](./BCP%20imgs/Leave%20%20.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  

# ***API*** 
   api/v2/crm/GetRequestByID?RequestID=e42c483f-529e-ee11-be37-0022489a5861

# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .


># ***BatchQueue:-***
- get list from crm / Getbyformrecid Params: EntityTypeRecId .
-  data will get it from local stroge

# ***API:-*** 
https://bcp.mawarid.com.sa/api/v1/entitytype/rulesdata/byformrecid?EntityTypeRecId

![](./BCP%20imgs/BatchQueue.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  

# ***API*** 


# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

># ***Leave Request Approval***

- get list from crm / Getbyformrecid Params: EntityTypeRecId .
-  data will get it from local stroge

# ***API:-*** 
https://bcp.mawarid.com.sa/api/v1/entitytype/rulesdata/byformrecid?EntityTypeRecId

![](./BCP%20imgs/BatchQueue.png)

# ***details*** 
  - button types will show based on condition 
  - if click details btn details will show in popup  

# ***API*** 


# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

># ***Termination Request Approval***

- get list from crm / Getbyformrecid Params: EntityTypeRecId .
-  data will get it from local stroge

# ***API:-*** 
https://bcp.mawarid.com.sa/api/v1/entitytype/rulesdata/byformrecid?EntityTypeRecId

![](./BCP%20imgs/BatchQueue.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  

# ***API*** 


# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

># ***Termination Request Approval***

![](./BCP%20imgs/Termination%20Request%20Approval.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  

# ***Workflow Details:-***
   Workflow action is 
   `ShowPending` ➠ `Draft` ➠ `Approved` ➠ `Reject` ➠ `ShowAll` 

  # ***API*** 
    https://bcp.mawarid.com.sa/api/v1/entitytype/batchqueue/byactionsstatus?actionStatus


# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

># ***Other Request Approval***
- get list from crm / Getbyformrecid Params: menuitem or customer name get in permission is true in get data .
-  data will get it from local stroge


# ***API:-*** 
https://bcp.mawarid.com.sa/api/v1/entitytype/productivitymenuitems?ispermission=true&customer-nam

![](./BCP%20imgs/BatchQueue.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  

# ***API*** 


# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

># ***Termination Request Approval:-***
get list from crm / Get request Params: activationrecordbylist or customer name  get from   local storage data  .
-  data will get it from local stroge.
   
# ***API:-***
   https://bcp.mawarid.com.sa/api/v1/entitytype/form/activationrecordbylist/111?customer-name

![](./BCP%20imgs/Termination%20Request%20Approval.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup  
# ***Workflow Details:-***
- Work flow base in actionStatus id based in work flow stages.
  ## ***API*** 
  https://bcp.mawarid.com.sa/api/v1/entitytype/batchqueue/byactionsstatus?actionStatus
 
   `ShowPending` ➠ `Draft` ➠ `Approved` ➠ `Reject` ➠ `ShowAll` 



# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

# ***Contract Renewal Request Approval:-***
-  get list from crm / Get request Params: activationrecordbylist or customer name  get from   local storage data  .
-  data will get it from local stroge.

  # ***API***:-   
https://bcp.mawarid.com.sa/api/v1/entitytype/rulesdata/byformrecid?EntityTypeRecId=112&FormRecId

![](./BCP%20imgs/Contract%20Renewal%20Request%20Approval.png)
# ***details*** 
  - button types will show based on condition 
  - if click details btn details will show in popup  
# ***Workflow Details:-***
- Work flow base in actionStatus id based in work flow stages.
  ## ***API*** 
  https://bcp.mawarid.com.sa/api/v1/entitytype/batchqueue/byactionsstatus?actionStatus
 
   `ShowPending` ➠ `Draft` ➠ `Approved` ➠ `Reject` ➠ `ShowAll`

   # ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file . 

 > #  ***Admin Request Approval:-***

 -  get list from crm / Get request Params: activationrecordbylist or customer name  get from   local storage data  .
-  data will get it from local stroge.

  # ***API***:-   

https://bcp.mawarid.com.sa/api/v1/entitytype/rulesdata/byformrecid?EntityTypeRecId=112&FormRecId

![](./BCP%20imgs/Admin%20Request%20Approval.png)

# ***details*** 
  -  button  types will show based on condition 
  - if click details btn details will show in popup .
   
# ***Workflow Details:-***

- Work flow base in actionStatus id based in work flow stages.
  ## ***API*** 

  https://bcp.mawarid.com.sa/api/v1/entitytype/batchqueue/byactionsstatus?actionStatus
 
   `ShowPending` ➠ `Draft` ➠ `Approved` ➠ `Reject` ➠ `ShowAll` 

   # ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

> # ***Letter Request Approval:-***
 -  get list from crm / Get request Params: activationrecordbylist or customer name  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
 https://bcp.mawarid.com.sa/api/v1/entitytype/form/activationrecordbylist/114?customer-name
 ![](./BCP%20imgs/Letter%20Request%20Approval.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
   
# ***Workflow Details:-***

- Work flow base in actionStatus id based in work flow stages.
  ## ***API*** 

  https://bcp.mawarid.com.sa/api/v1/entitytype/batchqueue/byactionsstatus?actionStatus
 
   `ShowPending` ➠ `Draft` ➠ `Approved` ➠ `Reject` ➠ `ShowAll` 

# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .
> # Reports:-

   > # Labor:-
   -  get list from crm / GetLaborListPaging Params: ProjectID based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
 https://bcp.mawarid.com.sa/api/v2/crm/GetLaborListPaging?ProjectID

# ***details*** 
  - button types will show based on condition 
  - if click details btn details will show in popup .
  - Labors list in loabor details and pasport setails expiry details in labor list.
  
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes , file .

> # ***Pay Statement Report:-***
   -  get list from crm / getReturnPayStatementNotHO Params: _payGroupID based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/getReturnPayStatementNotHO?_payGroupID

![](./BCP%20imgs/Pay%20Statement%20Report.png)
# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - Pay Statement in payGroupID based get in salary details working days , vacation , absent  and other details in get `payGroupID`.
  
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details , file .

># ***Salary And Fee Reports:-***
  
   -  get list from crm / GetTimeSheetTableList Params: _projId based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/GetTimeSheetTableList?_projId

![](./BCP%20imgs/Salary%20And%20Fee%20Reports.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - salary and report in Time Sheet Id based get in salary details working days , vacation , absent  and other details in get `_projId`.
  
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details , file .


># ***Loan Reports:-***
   -  get list from crm / getEmployeeLoanDetailsList Params: _projId based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/GetTimeSheetTableList?_projId

![](./BCP%20imgs/Loan%20Report.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - Loan reports  in projrctId based get in loan profile and other loandetails get 
  
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.


># ***Aging Report List:-***

   -  get list from crm / dynamicrestapicallfrombody Params: customer-name based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/dynamicrestapicallfrombody?customer-name

![](./BCP%20imgs/Aging%20Report%20List.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - aging report details Aging Period Definition	,   Description	, Company , Sys Operation Execution Mode details in aging report details.
  - Aging Period Definition and   company and other details.
  
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.

># ***All Invoice:-***
   -  get list from crm / getCustInvoiceJour Params: _custAccount or _projId based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/getCustInvoiceJour?_custAccount=CBN0002248&_projId

![](./BCP%20imgs/invioce.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - Loan reports list  in projrctId based get in 
   agent details
  - Aging Period Definition and   company and other details.
  
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.


# ***Pending Invoices:-***
   -  get list from crm / getPendingInvoices Params: _custAccount or _projId based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/getPendingInvoices?_custaccount=CBN0002248&_projId
![](./BCP%20imgs/)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  -  Pending Invoices  in custAccount or projId based get in 
   customer details
  -  pending invioce in Details Download,Summary,,DownLoad,AccountNum,CustName,Invoice and others details.
    
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.


># ***Account Statement:-***

 -  get list from crm / getCustStatement Params: _custaccount & page based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/getCustStatement?_custaccount=CBN0002248&$page

![](./BCP%20imgs/account%20statement.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - Account statement details Transfer date	,descrption,invoice,amount,Credit , debit	, and Amount balance details.
    
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.

># ***Account Statement Report:-***

 -  get list from crm / getCustStatement Params: _custaccount & customer-name based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/erp/getCustStatement?_custaccount=CBN0002248&customer-name

![](./BCP%20imgs/account%20statement%202.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - export button is export 	Date ,Invoice,Description	,Debit	, Credit and Balance details downlode in export.
  - Account statement report in debit and credit customer details.
    
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.

># ***Aging Report List:-***

 -  get list from crm / entitytyperulesdata Params: byformrecid or EntityTypeRecId based  get from   local storage data  .
-  data will get it from local stroge.
  
  # ***API***
https://bcp.mawarid.com.sa/api/v1/entitytype/rulesdata/byformrecid?EntityTypeRecId

![](./BCP%20imgs/aging%20report%20list%202.png)

# ***details*** 
  -  button types will show based on condition 
  - if click details btn details will show in popup .
  - aging report details Aging Period Definition	,   Description	, Company , Sys Operation Execution Mode details in aging report details.
  - Aging Period Definition and   company and other details.
    
# ***General Notes*** 
  -  createing notes in we get below fields Title , notes salary details and file details.









 

    