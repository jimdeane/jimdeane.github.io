CREATE USER [jimd@malue.co.uk] FROM EXTERNAL PROVIDER;
CREATE USER [coenraadm@malue.co.uk] FROM EXTERNAL PROVIDER;
CREATE USER [sergeya@malue.co.uk] FROM EXTERNAL PROVIDER;

ALTER ROLE db_owner ADD MEMBER [jimd@malue.co.uk]; 
ALTER ROLE db_owner ADD MEMBER [coenraadm@malue.co.uk]; 
ALTER ROLE db_owner ADD MEMBER [sergeya@malue.co.uk]; 