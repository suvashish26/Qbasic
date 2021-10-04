# Qbasic
Qbasic

Reverse
declare function rev$(a$)
Cls

Input "enter any name"; a$
Print rev$(a$)
If a$ = rev$(a$) Then
    Print "its palindrom"
Else
    Print "its not palindrome"
End If

End
Function rev$ (a$)

    For i = Len(a$) To 1 Step -1
        nana$ = Mid$(a$, i, 1)
        c$ = c$ + nana$
    Next i
    rev$ = c$
End Function

declare sub rev(a$)
Cls
Input "enter"; a$
Call rev(a$)
End
Sub rev (a$)
    For i = Len(a$) To 1 Step -1
        x$ = Mid$(a$, i, 1)
        w$ = w$ + x$
    Next i
    Print "the value is "; w$
    If w$ = a$ Then
        Print "its a palindrome"
    Else
        Print "its not"
    End If

declare function vow(a$)
Cls
Input a$
Print vow(a$)
End
Function vow (a$)
    c = 0
    For i = 1 To Len(a$)
        w$ = UCase$(Mid$(a$, i, 1))
        If w$ = "A" Or w$ = "E" Or w$ = "O" Or w$ = "U" Or w$ = "I" Then
            c = c + 1
        End If
    Next i
    vows = c
End Function

declare sub vow(a$)
Cls
Input a$
Call vow(a$)
End
Sub vow (a$)
    c = 0
    For i = 1 To Len(a$)
        w$ = UCase$(Mid$(a$, i, 1))
        If w$ = "A" Or w$ = "E" Or w$ = "O" Or w$ = "U" Or w$ = "I" Then
            c = c + 1
        End If
    Next i
    Print "the vowels are"; c
End Sub

declare function pro(a)
Cls
Input a
Print pro(a)
End
Function pro (a)
    s = 1
    While a <> 0
        r = a Mod 10
        s = s * r
        a = a \ 10
    Wend
    pro = s
End Function

declare function alt$(a$)
Cls
Input "enter name"; a$
Print alt$(a$);
End
Function alt$ (a$)
    For i = 1 To Len(a$)
        x$ = Mid$(a$, i, 1)
        If i Mod 2 = 0 Then
            Print LCase$(x$)
        Else
            Print UCase$(x$)
        End If
        z$ = z$ + x$
    Next i
End Function
End Sub

declare function oct(a)
Cls
Input a
Print oct(a)
End
Function oct (a)
    While a <> 0
        r = a Mod 8
        s$ = Str$(r) + s$
        a = a \ 8
    Wend
    v = Val(s$)
    oct = v
End Function
Rem oct to dec

declare sub bin(a)
Cls
Input a
Call bin(a)
End
Sub bin (a)
    While a <> 0
        r = a Mod 16
        If r = 10 Then
            B$ = "A"
        ElseIf r = 11 Then
            B$ = "B"
        ElseIf r = 12 Then
            B$ = "C"
        ElseIf r = 13 Then
            B$ = "D"
        ElseIf r = 14 Then
            B$ = "E"
        ElseIf r = 15 Then
            B$ = "F"
        End If

        s$ = Str$(r) + s$
        a = a \ 16
    Wend
    Print "hex is "; s$
End Sub


declare sub pattern
cls
call pattern
end
sub pattern
a = 1
b= 1

for i = 1 to 9
c = a+b
Print c
a=b
b=c
next i
end sub

declare function prime (A)
Cls
Input A
p = prime(A)
Print "total num of factors = "; p
If p = 2 Then ' total number of prime are only two
    Print "prime"
Else
    Print "not prime"
End If

End

Function prime (A)
    count = 0
    For i = 1 To A
        If A Mod i = 0 Then
            count = count + 1 ' 1 factor
        End If
    Next i
    prime = count
End Function

Function revNum (a)
    While a <> 0
        r = a Mod 10 ' takes ot the last digit
        c = c * 10 + r '' stoes first digit suppose in 123 its 3 then next time 3*10 +2 32 and it reverses
        a = a \ 10 '' here it terminates 123/10 is 12.3 so 3 is gone and 12 remains
    Wend
    revNum = c
End Function

DECLARE FUNCTION ARMST (N)
Cls
Input "ENTER ANY NUMBER"; N
A = N 'before a becomes 0 storing the vaue of original number
AR = ARMST(N)
If A = AR Then
    Print A; "IS ARMSTRONG NUMBER"
Else
    Print A; "IS NOT ARMSTRONG NUMBER"
End If
End

Function ARMST (N)
    S = 0
    While N <> 0 ' until 0
        R = N Mod 10
        S = S + R ^ 3
        N = N \ 10
    Wend
    ARMST = S
End Function
'output = 153 = (1*1*1)+(5*5*5)+(3*3*3)

DECLARE SUB Count(s$);
Cls
Input "Enter string:"; s$
Call Count(s$)
End
Sub Count (s$)
    wcount = 1
    For i = 1 To Len(s$)
        b$ = Mid$(s$, i, 1)
        If b$ = " " Then
            wcount = wcount + 1
        End If
    Next i
    Print "The total word is: "; wcount
End Sub

CLS
s$ = "NEPAL"
t = 3
FOR i = LEN(s$) TO 1 STEP -1

PRINT TAB(t); MID$(s$, i, 1)
t = t + 1
NEXT i
END
String Pattern in QBasic
2 Comments.

 

String Pattern
N
NE
NEP
NEPA
NEPAL

CLS

A$="NEPAL"

FOR I = 1 TO LEN (A$)

PRINT LEFT$(A$,i)

NEXT i

END

Display

NEPAL
NEPA
NEP
NE
N

CLS

A$ = "NEPAL"

FOR i = LEN(A$) TO 1 STEP -1

PRINT RIGHT$(A$, i)

NEXT i

END

Display:

PROGRAMMING
PROGRAMMIN
PROGRAMMI
PROGRAMM
PROGRAM
PROGRA
PROGR
PROG
PRO
PR
P

CLS
s$ = "PROGRAMMING"
t = 1
r = 1
FOR i = LEN(s$) TO 1 STEP -1
PRINT TAB(t); MID$(s$, r, i)
NEXT i
END




Display: 

PROGRAMMING
ROGRAMMING
OGRAMMING
GRAMMING
RAMMING
AMMING
MMING
MING
ING
IN
G

CLS
s$ = "PROGRAMMING"
t = 1
r = 1
FOR i = LEN(s$) TO 1 STEP -1
PRINT TAB(t); MID$(s$, r, i)

r = r + 1
NEXT i
END

 

Display

L
AL
PAL
EPAL
NEPAL

CLS

A$ = "NEPAL"

FOR I = 1 TO LEN(A$)

PRINT RIGHT$(A$, I)

NEXT I

END

 

 

Display

NE

           EP

                       PA

                                AL

CLS
a$ = "NEPAL"
x = LEN(a$)
FOR i = 1 TO x – 1
PRINT TAB(i); MID$(a$, i, 2)
NEXT i
END

 

Display

P

EPA

NEPAL

CLS
s$ = "NEPAL"
C = 1: b = 35
FOR i = 3 TO 1 STEP -1
PRINT TAB(b); MID$(s$, i, C)
C = C + 2
b = b – 1
NEXT i
END




Display

L

    A

        P

              E

                  N

CLS
s$ = "NEPAL"
t = 3
FOR i = LEN(s$) TO 1 STEP -1

PRINT TAB(t); MID$(s$, i, 1)
t = t + 1
NEXT i
END

Display

                                                        L

                                              A

                                     P

                            E

                  N

CLS
s$ = "NEPAL"
t = 8
FOR i = LEN(s$) TO 1 STEP -1

PRINT TAB(t); MID$(s$, i, 1)
t = t – 1
NEXT i
END

Display

                                                         N

                                             E

                                     P

                            A

                  L

CLS
s$ = "NEPAL"
t = 8
FOR i = 1 TO LEN(s$)

PRINT TAB(t); MID$(s$, i, 1)
t = t – 1
NEXT i
END

Display

N

     E

          P

               A

                        L

 

CLS
s$ = "NEPAL"
t = 8
FOR i = 1 TO LEN(s$)

PRINT TAB(t); MID$(s$, i, 1)
t = t + 1
NEXT i
END

Display

N

E

P

A

L

CLS
s$ = "NEPAL"

FOR i = 1 TO LEN(s$)

PRINT MID$(s$, i, 1)

NEXT i
END

Display

L

A

P

E

N

CLS
s$ = "NEPAL"

FOR i = LEN(s$) TO 1 STEP -1

PRINT MID$(s$, i, 1)

NEXT i
END

Display:

*
**
***
****
*****
*
**
***
****
*****
*
*
*
*
*

CLS
A$ = “*********”
A = 1
B = 1
FOR I = 1 TO 5
COLOR 4
PRINT MID$(A$, A, B)
B = B + 1
NEXT I
A = 1
B = 1
FOR J = 1 TO 5
COLOR 6
PRINT MID$(A$, A, B)
B = B + 1
NEXT J
FOR K = 1 TO 5
COLOR 5
PRINT MID$(A$, K, 1)
NEXT K
END




Display

*
**
***
****
*****

CLS

A$=”****”

FOR I = 1 TO LEN (A$)

PRINT LEFT$(A$,i)

NEXT i

END

OR

CLS
A$ = "*********"
A = 1
B = 1
FOR I = 1 TO 5
PRINT MID$(A$, A, B)
B = B + 1
NEXT I
END

Display

*****
****
***
**
*

CLS

A$ = "*****"

FOR I = LEN(A$) TO 1 STEP -1

PRINT LEFT$(A$, I)

NEXT I

END

OR

CLS
A$ = "*********"
A = 1
B = 5
FOR I = 5 to 1 step -1
PRINT MID$(A$, A, B)
B = B -1
NEXT I
END

R

GRA

OGRAM

ROGRAM

PROGRAM

CLS
s$ = "PROGRAM"
c = 1: b = 40
FOR i = 5 TO 1 STEP -1
PRINT TAB(b); MID$(s$, i, c)
c = c + 2
b = b – 1
NEXT i
END
