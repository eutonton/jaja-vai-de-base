# jaja-vai-de-base

<?PHP
// echo "<h1>Tipos de dados escalares</h1><br>";
// echo "<hr>";

// $nome = ["Fabio","João","Matheus"];
// print_r($nome);

echo "<h1>String</h1><br>";
echo "<hr>";

$nome1 = "tonton";
var_dump($nome1);
if(is_string($nome1."<br>")):
    echo "É uma string";
else:
    echo "Não é uma string";
endif;

echo "<hr>";
$nome2 = 10;
var_dump($nome2);
if(is_int($nome2)):
    echo "É um inteiro";
else:
    echo "Não é um inteiro";
endif;

echo "<hr>";
$nome3 = 1200.81;
var_dump($nome3);
if(is_float($nome3)):
    echo "É um Decimal";
else:
    echo "Não é um Decimal";
endif;

echo "<hr>";
echo "<h1>Float - Tratamento para trazer os zeros nos valores</h1><br>";

$salario = 1200.00;
var_dump($salario);

if(is_float($salario)){
    $salarioFormatado = number_format($salario,2, ',','.');
    echo "Salario: R$ ". $salarioFormatado;
}else {
    echo "Não é um valor float";
}

echo"<hr>";
echo"<h1>Tipos de dados compostos</h1><br>";

echo"<h1>Array</h1><br>";

$nome = ["Fabio","João","Matheus"];
var_dump($nome);
print "<br>";
$diversos = ["Fabio",2,10.5];
var_dump($diversos);


?>
