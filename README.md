# logical-operators

=>The purpose of Logical Operators is that "To combine Two OR More Relational Expressions."
=>If Two OR More Relational Expressions combined with  Logical Operators then It is called Logical Expression.
=>The Result of Logical Expression is either True or False.
=>The Logical Expression is also Compound Test Cond and whose result can be either True or False.
=>In Python Programming, we have 3 Types of  Logical Operators. They are given in the following Table.

They are 3 logical operators
1)and
2)or
3)not

1)and operator:
=>Syntax:    RelExpr1  and  RelExpr2
eg-1:
>>> True and False---------------False
>>> False and True---------------False
>>> False and False-------------False
>>> True and True----------------True

>>> Examples-2
------------------------------
>>> 10>2 and 20>4------------------------True----Full length evaluation
>>> 10>3 and 20>4 and 40>5----------True----Full length evaluation
>>> 10>20 and 20>3----------------------False---Short Circuit Evaluation
>>> 10>20 and 30>3 and 40>30-------False---Short Circuit Evaluation
>>> 10>2 and 20>30 and 40>3--------False---Short Circuit Evaluation
------------------------------------------------------------------------------------------------
Short Circuit Evaluation in the case of 'and' Operator
------------------------------------------------------------------------------------------------
=>If Two OR More Relational Expressions Connected with Logical Operator  (called Logical Expression) 'and' If the Result of Initial Relational Expression is False  then PVM will not evaluate Rest of Relational Expression and final the Result of Entire Logical Expression is False. This Process of Evaluation is Called Short Circuit Evaluation

Special Points about 'and' Operator--Most IMP
*********************************************************************
>>> 100 and 200------------------------200
>>> -100 and -200----------------------200
>>> 0 and 30----------------------------0
>>> 100 and 0--------------------------0
>>> 100 and 200 and 300-----------300
>>> 100 and 0 and 400--------------0
>>> "False" and "True"-------------'True'
>>> "True" and "False"------------'False'
>>> "Java" and "Python"----------'Python'
>>> 0b1010 and 0xF----------------15
>>> "True" and bool("False")-------------True
>>> bool("") and True-----------------------False

--------------------------------------------
2. or Operator
***************************************
=>Syntax:    RelExpr1  or  RelExpr2

Example-1
--------------------------
>>> True or False----------------True
>>> False or True----------------True
>>> False or False--------------False
>>> True or True-----------------True
--------------------------
Example-2
--------------------------
>>> 10>2 or 20>30-------------------------True------Short Circuit Evaluation
>>> 10>20 or 30>40-----------------------False----Full length evaluation
>>> 10>2 or 40>20 or 50>100----------True------Short Circuit Evaluation
>>> 10>20 or 40>50 or 50>60----------False----Full length evaluation
>>> 10>20 or 40>30 or 50>60----------True------Short Circuit Evaluation
---------------------------------------------------------------------------------------------------------------
Short Circuit Evaluation in the case of 'or' Operator
---------------------------------------------------------------------------------------------------------------
=>If Two OR More Relational Expressions Connected with Logical Operator (called Logical Expression) 'or' If the Result of Initial Relational Expression is True  then PVM will not evaluate Rest of Relational Expression and final the Result of Entire Logical Expression is True. This Process of Evaluation is Called Short Circuit Evaluation
--------------------------------------------------------------------------------------------------------------------------------------------------------------
Special Points about 'or' Operator--Most IMP
*********************************************************************
>>> 10 or 20------------------------10
>>> 0 or 20-------------------------20
>>> 20 or 0------------------------20
>>> 10 or 20 or 30--------------10
>>> "Python" or "java" or "C"------------'Python'
>>> "Python" or False or True-----------'Python'
---------------------------------------------------------------------------------------------------------------
Special Points about  'and'   and   'or'  Operator--Most IMP
NOTE: We must First Evaluate 'and' , later evaulate 'or' bcoz 'and' operator is having More Priority than 'or'
********************************************************************************
>>> 10 or 20 and 40-----------------10
>>> 20 and 40 or 30-----------------40
>>> 10 and 30 and 20 or 50 and 60 or 70----------20
********************************************************************************
3. not Operator
***************************************
Syntax:		not RelExpr
          not Logical Expr

Exanples
--------------------------------
>>> not True----------------False
>>> not False--------------True
>>> not 10-------------------False
>>> not 0--------------------True
>>> not "Python"----------False
>>> not ""--------------------True
>>> not 10>20-------------True
>>> not 20>10-------------False
>>> not(10>2 or 20>30)------False
>>> not(10>2 and 20>30)----True
