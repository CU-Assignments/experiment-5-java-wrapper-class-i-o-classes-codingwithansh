import java.util.ArrayList;
import java.util.List;

public class AutoBoxingExample {
    public static void main(String[] args) {
        List<Integer> numbers = new ArrayList<>();
        numbers.add(10);  
        numbers.add(20);
        numbers.add(30);
        numbers.add(parseStringToInteger("40"));
        numbers.add(parseStringToInteger("50"));
        int sum = calculateSum(numbers);
        System.out.println("Sum of numbers: " + sum);
    }
    public static Integer parseStringToInteger(String str) {
        return Integer.parseInt(str); 
    }
    public static int calculateSum(List<Integer> numbers) {
        int sum = 0;
        for (Integer num : numbers) {
            sum += num; 
        }
        return sum;
    }
}


