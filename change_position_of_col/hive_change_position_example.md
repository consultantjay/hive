

Example:

<code> 
CREATE TABLE test_change (a int, b int, c int);
 
<B>  First change column a's name to a1.</B>

ALTER TABLE test_change CHANGE a a1 INT;
 
<B> Next change column a1's name to a2, its data type to string, and put it after column b.</B>

ALTER TABLE test_change CHANGE a1 a2 STRING AFTER b;

<B>  The new table's structure is:  b int, a2 string, c int.</B>
  
<B>  Then change column c's name to c1, and put it as the first column.</B>

ALTER TABLE test_change CHANGE c c1 INT FIRST;

<B>  The new table's structure is:  c1 int, b int, a2 string.</B>
  
<B>  Add a comment to column a1</B>

ALTER TABLE test_change CHANGE a1 a1 INT COMMENT 'this is column a1';
</code>



