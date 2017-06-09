# MVCAudit
c# MVC Audit


### auditing are pupuler issue to track the data in website , who change data  , when data changed , what are the old values are ???!! 
# Setup 

## SQL 

### 1- UserTable -> 
      ID int ,
      UserName nvarchar(50), 
      Password nvarchar(50),
      EMailAddress nvarchar(50),
      LastLogin DateTime,
      IsActive bit
      
### 2- Audit Table
      ID    int    
      FIled    int    
      ActionEnum    int   
      EditTime    datetime    
      DataModel    nvarchar(Max)   
      Changes    nvarchar(MAX)    
      ValueBefore    nvarchar(MAX)   
      ValueAfter    nvarchar(MAX)   
      
# Models

## 1- UserTable Model 
        public class SampleDataModel
        {
        public int ID { get; set; }
        public string UserName { get; set; }
        public string Password { get; set; }
        public DateTime LastLogin { get; set; }
        public bool Deleted { get; set; }
         public bool IsActive { get; set; }
        .......
        }
        

