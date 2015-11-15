# php-format

## getting started  
``` 
include 'Format.php';  
use Prototypeblocks\Format;  
``` 
## examples  
#### arrayToJson
``` 
$array = array('a','b','c');
$json = Format::arrayToJson($array);
// $json is $array converted into JSON format
``` 
#### arrayToString
``` 
$array = array('a','b','c');
$string = Format::arrayToString($array);
// $string is imploded array, default delimiter is ' ' 
``` 
``` 
$array = array('a','b','c');
$string = Format::arrayToString($array, '-');
// $string is imploded array with delimiter '-'
``` 
#### csvToArray
``` 
$csv = '';
$array = Format::csvToArray($csv);
// $array is CSV converted to array
``` 
#### jsonToArray
``` 
$json = '';
$array = Format::jsonToArray($json);
// $array is JSON string converted to array
``` 
#### stringToArray
``` 
$string = 'This is a normal string';
$array = Format::stringToArray($string);
// $array is exploded string, default delimiter is ' ' 
``` 
``` 
$string = 'This is a normal string, with a - for some weird reason';
$array = Format::stringToArray($string, '-');
// $array is exploded string with delimiter '-'
``` 
#### toBool  
Alias for Format::toBoolean  
#### toBoolean  
``` 
$var = ?
$boolean = Format::toBoolean($var);
// $boolean is $var converted to boolean
``` 
#### toFloat  
``` 
$number = 15;
$float = Format::toFloat($number);
// $float is $number converted to float
``` 
#### toInt  
Alias for Format::toInteger
#### toInteger  
``` 
$number = 15.50;
$integer = Format::toInteger($number);
// $integer is $number converted to integer
``` 
#### toJson  
``` 
$var = ?
$json = Format::toJson($var);
// $json is $var converted to JSON format
``` 
#### toString  
``` 
$var = ?
$string = Format::toString($var);
// $string is $var converted to string
``` 
#### objectToArray
``` 
$object = \stdClass;
$array = Format::objectToArray($object);
// $array is $object converted to array (recurisve)
``` 
#### arrayToObject
``` 
$array = array();
$object = Format::arrayToObject($array);
// $object is $array converted to object
``` 
#### objectToJson
``` 
$object = \stdClass;
$json = Format::objectToJson($object);
// $json is $object converted to JSON format
``` 
#### toObject  
``` 
$var = ?
$object = Format::toObject($var);
// $object is $var converted to object
``` 
#### toArray  
``` 
$var = ?
$array = Format::toArray($var);
// $array is $var converted to array
``` 
#### xmlToArray
``` 
$xml = '';
$array = Format::xmlToArray($xml);
// $array is $xml converted to array
``` 
