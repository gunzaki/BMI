# BMI

public class Main {

    public static float calculateBmi(double height, double weight) {
        return (float) (weight / (height * height));
    }

    public static String getBmiCategory(double bmi) {
        if (bmi < 18.5) return "Underweight";
        else if (bmi < 24.9) return "Normal weight";
        else if (bmi < 29.9) return "Overweight";
        else return "Obese";
    }

    public static void main(String[] args) {
        var height = 2.0;
        var weight = 75.0;

        var bmi = calculateBmi(height, weight);
        var category = getBmiCategory(bmi);

        System.out.println("BMI: " + bmi);
        System.out.println("Category: " + category);
    }
}