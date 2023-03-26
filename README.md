# g-code_regualr_expressions
An unorganized collection of expressions used to find patterns in g-code.


(G|M|X|Y|Z|I|J|K|F)(?<val>-?\d*\.?\d+\.?)
([A-z])(?<val>-?\d*\.?\d+\.?)
[^GMgm0-9](?:-?\d*\.?\d+\.?)
 (?i)[G](1)?5[4-9](.1)?\\s?(P[0-9]{1,3})?
([Gg]0?[01]) *(([XxYyZz]) *(-?\d+.?\d*)) *(([XxYyZz]) *(-?\d+.?\d*))? *(([XxYyZz]) *(-?\d+.?\d*))?
(?<x>:-?\d+.\d+) (?<y>:-?\d+.\d+) (?<z>:-?\d+.\d+) (?<e>:-?\d+.\d+) .*
(?<x>-?\d+\.\d+),(?<y>-?\d+\.\d+),(?<z>-?\d+\.\d+),(?<rotation>-?\d+\.\d+)
 (?i)[G]1[1-2][0-9] 
  (?i)[G][0-9]{1,3}(\\.[0-9])?
  (?i)[M][0-9]{1,3}
  (\\+|\\*|\\/|\\*\\*)
  (?i)([S])\\s?(\\d+|(?=[#\\[]))
  (?i)([IJK])(\\-?\\d*\\.?\\d+\\.?|\\-?\\.?(?=[#\\[]))
  
(?i)(GOTO\\s?\\d+)
\\(.+\\
(\\(.+\\))  
(?i)(EQ|NE|LT|GT|LE|GE|AND|OR|XOR)
(?i)(DO\\s?\\d*|WHILE|WH|END|IF|THEN|ELSE|ENDIF)  
  
  
  


