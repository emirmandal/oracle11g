# oracle11g

sqlplus / as sysdba


Verify Database

select name from v$database;
select name from v$controlfile;
select name from v$datafile;
select * from dual;
select sysdate from dual;


Database Startup

startup nomount     - nomoun stage
startup mount       - mount stage
startup             - open stage


Database Shutdown

shutdown immediate         - active transactions trminated, uncommitted changes rolled back
shutdown transactional     - ait for all transactions to complete, dont allow new
shutdown normal            - wait for all users to disconnect
shutdown abort             - fastest shutdown mode

