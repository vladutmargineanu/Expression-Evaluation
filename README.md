# Expression-Evaluation
Homework for the Introduction to Computer Organization and Assembly Language @ ACS, UPB 2018

# Algorithm

Expression evaluation in postfixed Polish form

 Se citeste de la `stdin` stringul ce contine expresia, iar adresa acestuia se stocheaza in `ecx`. Dupa care se parcurge stringul caracter cu caracter si se efectueaza operatiile gasite sau se formeaza numere, prin intermediul functiei `number_construction`. Aceasta nu primeste parametri, operand cu acelasi registru `ecx` ca si main-ul si returneaza numarul creat fara semn in `eax`. Nu este nevoie de variabile suplimentare, in afara de stringul pentru input si a stivei, toate operatiile fiind efectuate cu registrele.

# Implementation:

S-a folosit stiva sistemului pentru a memora numerele citite si rezultatele in urma efectuarii calculelor.
Se retine ultimul numar obtinut din calcule sau din parsarea inputului in 'eax'. Restul rezultatelor se retin pe stiva sistemului.
Registrul 'exc' creste pana cand valoarea de la adresa acestuia este '0', corespuznator cu terminatorul de sir '\0'.

