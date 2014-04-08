<?php
$a=array(
1=>array(101,'sanjay','karonjiya'),
2=>array(102,'atul','vishwakarma'),
3=>array(103,'sachin','patil')
);

foreach($a as $v)
{
  $as=array();
 foreach($v as $V)
 {
 is_string($V)?$as[]="'$V'":$as[]=$V;
 }
 echo "insert into users values (".implode(',',$as).")";
 echo"<br>";
}



?>
