# Homeworks1-2


###Придумать и написать любой пример использования if-elseif-else.



        if(date(m) == 12||01||02){
            echo "Зима нынче :)";
        }elseif (date(m) == 03||04||05){
            echo "Весна нынче:)";
        }elseif(date(m) == 06||07||03){
            echo "Осень нынче :)";
        }else{
            echo "Летушко:)";
        }
        
        



###Переписать скрипт оператора switch->case->break так, чтобы использовалась конструкция if->elseif->else.

    switch ($mark) {
        case 2:
            echo "I am better!!";
            break;
        case 3:
            echo "OK :(";
            break;
        case 4:
            echo "I am good :)";
            break;
        case 5:
            echo "YeeeeWhaaaa!!!!";
            break;
    }

    */


    if($mark==2){
        echo "I am better!!";
    }elseif ($mark==3) {
        echo "OK :(";
    }elseif ($mark==4) {
        echo "I am good :)";
    }else {
        echo "YeeeeWhaaaa!!!!";
    }
    echo "\n";
    /////////////////////////////////
    //3)
    //Переписать скрипт оператора if->elseif->else так, чтобы использовалась конструкция switch->case->break.
    //Переменные взяты с fizz-bizz задачи.

    switch (isset($result[0]) && isset($result[1])){
        case ($i%$result[0]==0 && $i%$result[1]==0):
            echo "FB ";
            break;
        case ($i%$result[0]==0):
            echo "F ";
            break;
        case ($i%$result[1]==0):
            echo "B ";
            break;
        case true:
            echo $i." ";
            break;
    }


###Придумать и написать любой пример использования тернарного оператора.

     print (date(s) <=15) ? " Твоя скорость в пределах нормы = ".date(s)."км/ч"
        ?:(date(s) <=30) ?: " Твоя скорость в пределах нормы = ".date(s)."км/ч"
        ?:(date(s) <=45) ?: " Осторожно !!! ".date(s)."км/ч"
        ?:(date(s) <=60) : "Превышение скорости!!!!!!!! " .date(s)."км/ч";

    //?






###ЗАДАЧА FIZZ-BIZZ
            $handle = fopen("php://stdin","r");
            $mark = fgets($handle);
            $result = explode(" ", $mark);

            for ($i = 1; $i <= $result[2]; $i++) {

            if ($i % $result[0] == 0 && $i % $result[1] == 0) {
                echo "FB ";

            } elseif ($i % $result[0] == 0) {
                echo "F ";
            } elseif ($i % $result[1] == 0) {
                echo "B ";
            } else {
                echo $i . " ";
            }

            }










