# 12-01_BD
1. Сотрудники  
•  Идентификатор, первичный ключ serial,  
•  Фамилия: varchar(50)  
•  Имя: varchar(50)  
•  Отчество: varchar(50),  
•  Дата приема на работу (Date),  
•  Должность_id: внешний ключ, integer  -- на табл должности  
•  Подразделение_id: внешний ключ, integer  -- на табл структурные подразделения   
•  Проект_id:   внешний ключ, integer  --  на табл проекты

2. Должность  
•  Идентификатор, первичный ключ serial,  
•  Должность, varchar(100)
•  Оклад (DECIMAL 10, 2), оклад id (integer)

4. Структурные подразделения  
•  Идентификатор, первичный ключ serial,  
•  название, varchar(100)  
•  тип_id внешн ключ integer  -- на табл типы подразд 

5. Тип подразделения  
•  Идентификатор первичный ключ serial,  
•  Полное наименование структурного подразделения, varchar(100)  

6. Адреса филиалов  
•  Идентификатор первичный ключ serial,  
•  город_id:  внешний ключ, integer  --  на табл города  
•  регион_id:  внешний ключ, integer  --  на табл регион  
•  Полный адрес филиала, varchar(255)  

7. Проект  
•  Идентификатор первичный ключ serial,  
•  Название проекта, varchar(100)    

8. Оклад  
•  Идентификатор первичный ключ serial,    
•  Идентификатор_сотрудника_id (integer)  

9. Города
•  Идентификатор первичный ключ serial,  
•  название, varchar(100)  
•  регион_id: внешн ключ integer  -- на табл регионы  

10. Регионы
•  Идентификатор первичный ключ serial,  
•  название, varchar(100)  
