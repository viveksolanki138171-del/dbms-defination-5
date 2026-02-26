# dbms-defination-5
--Write a PL/SQL block that calculates the simple interest based on given principal amount, rate of interest and number of years.


set serveroutput on; declare
v_principal number; v_rate		number; v_years			number; v_si	number;

begin

v_principal := &enter_principal; v_rate	:= &enter_rate; v_years		:= &enter_years;

v_si := (v_principal * v_rate * v_years) / 100;


dbms_output.put_line('principal amount : ' || v_principal); dbms_output.put_line('rate of interest : ' || v_rate); dbms_output.put_line('number of years : ' || v_years); dbms_output.put_line('simple interest : ' || v_si);

end;
/
