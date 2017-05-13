<?php
$con=mysql_connect("sql208.adfreehost.ir","adfr_20066596","s5f4062v");
mysql_select_db(adfr_20066596_noun,$con);
$response=array();
$result=mysql_query("select * from bread");
if(mysql_num_rows($result)>0){
while($row=mysql_fetch_array($result)){
$temp=array();
$temp["name"]=$row["name"];
$temp["phone"]=$row["phone"];
$temp["address"]=$row["address"];
$temp["count"]=$row["count"];
$temp["breadtype"]=$row["breadtype"];
$response["bread"]=array();
array_push($response["bread"],$temp);
echo json_encode($response);
}
$response["t"]=1;
echo json_encode($response);
}else{
$response["t"]=0;
$response["message"]="not found";
echo json_encode($response);
echo json_encode($response);
}
?>
