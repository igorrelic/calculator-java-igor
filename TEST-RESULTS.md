# Rezultati Black box testiranja

| Testirano     	| Ocekivano        	| Dobijeno                        	| Test prošao 	|
|---------------	|------------------	|---------------------------------	|-------------	|
| 5+5           	| 10               	| 10                              	| Da          	|
| 5-5           	| 0                	| 0                               	| Da          	|
| 5*5           	| 25               	| 25                              	| Da          	|
| 5/5           	| 1                	| 1                               	| Da          	|
| 4+5*6         	| 36               	| 36                              	| Da          	|
| 7-10/2        	| 2                	| 2                               	| Da          	|
| 5*5-5/5+5     	| 29               	| 29                              	| Da          	|
| -5+7          	| 2                	| 2                               	| Da          	|
| -5-5          	| -10              	| -10                             	| Da          	|
| -5*5          	| -25              	| -25                             	| Da          	|
| -5*-5         	| error            	| error                           	| Da          	|
| -5/5          	| -1               	| -1                              	| Da          	|
| 5++5          	| error            	| error                           	| Da          	|
| 5--5          	| error            	| error                           	| Da          	|
| 5**5          	| error            	| error                           	| Da          	|
| 5//5          	| error            	| error                           	| Da          	|
| 5+/5          	| error            	| error                           	| Da          	|
| 5/0           	| infinity         	| infinity                        	| Da          	|
| 5*0           	| 0                	| 0                               	| Da          	|
| aa+8          	| error            	| error                           	| Da          	|
| bb/5          	| error            	| error                           	| Da          	|
| cc+/10        	| error            	| error                           	| Da          	|
| prazan unos   	| error            	| StringIndexOutOfBoundsException 	| Ne          	|
| 5   +    5    	| 10               	| 10                              	| Da          	|
| 5+5-          	| error/upozorenje 	| 10                              	| Ne (mozda)  	|
| -10           	| -10              	| -10                             	| Da          	|
| 5+-5          	| 0                	| error                           	| Ne          	|
| 5+(-5)        	| 0                	| error                           	| Ne          	|
| 1/3           	| oko 0.33333333   	| 0.33333334                      	| Da          	|
| 1/5           	| 0.2              	| 0.2                             	| Da          	|
| 12.35 + 18.68 	| 31.03            	| 31.03                           	| Da          	|





# Jedinični test
import java.util.ArrayList;

import java.util.List;

public class CalculatorTest {

    public static void main(String[] args) {
        List<Float> numbers = new ArrayList<>();
        numbers.add(5.0f);
        numbers.add(3.0f);

        List<String> operations = new ArrayList<>();
        operations.add("+");

        Calculator.Calculate(numbers, operations);

        float expected = 8.0f;
        float actual = Calculator.finalResult;

        if (expected == actual) {
            System.out.println("Test passed.");
        } else {
            System.out.println("Test failed. Expected: " + expected + ", but got: " + actual);
        }
    }
}
