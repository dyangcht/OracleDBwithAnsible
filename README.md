# OracleDB with Ansible 單機版安裝自動化

要安裝前如果有不熟悉怎麼安裝甲骨文資料庫的，請參考甲骨文資料庫的安裝手冊,在這兒 
(https://docs.oracle.com/en/database/oracle/oracle-database/19/ladbi/index.html)

環境說明: 
作業系統: Red Hat Enterprise Linux 7.8 
Ansible: ansible 2.9.6

在安裝前請先到甲骨文官網 OTN 下載必要之軟體，此範例是安裝 Oracle Database 19c 64 bit (LINUX.X64_193000_db_home.zip). 要能從官網下載需要先註冊，當然它是免費註冊的哦～

### 事前準備：
1. Ansible
2. Oracle Database 19c (64 bit) binary file: LINUX.X64_193000_db_home.zip
3. Red Hat Enterprise Linux 7.x 64 bit
4. 公鑰和私鑰一對

### 檔案解說
```
rm.yml: 清除前一次測試留下的檔案，以利下次測試用 (house keeping)
oracle19c_install.yml: 從安裝到建資料庫一次完成
without_cp_bin.yml: 不安裝軟體，只建使用者及資料庫；因為安裝軟體很花時間，測試時可以加快一點速度
```

```
Coding here
```
