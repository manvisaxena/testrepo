###STEPS-:

>1. Run this command to change the **birth_date column to second place** along with ' ' :
>`%s/\v^(\S*)\s(\S*)\s(\S*)\s(\S*)\s(\S*-*-*)\s(\S*-*-*)/\1,'\5','\2','\3','\4','\6'`

> 2. To change **Female to F** and **Male to M**-:
> * `%s/Female/F/g`
> * `%s/Male/M/g`

> 3. To insert query line at the beginning-:
> `%s/^/insert into employees(emp_no,birth_date,first_name,last_name,gender,hire_date)values(/g`

> 4. To insert closing brackets at the end-:
> `%s/$/);/g`

