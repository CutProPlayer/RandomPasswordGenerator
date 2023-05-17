# RandomPasswordGenerator
RandomPasswordGenerator
import java.util.Random;

public class RandomPasswordGenerator {
    public static void main(String[] args) {
        int length = 8;
        String password = generatePassword(length);
        System.out.println("Сгенерированный пароль: " + password);
    }

    public static String generatePassword(int length) {
        String characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()";
        StringBuilder password = new StringBuilder();

        Random random = new Random();
        for (int i = 0; i < length; i++) {
            int index = random.nextInt(characters.length());
            password.append(characters.charAt(index));
        }

        return password.toString();
    }
}
