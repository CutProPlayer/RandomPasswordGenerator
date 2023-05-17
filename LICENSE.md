 int length = 8;
        String password = generatePassword(length);
        System.out.println("Сгенерированный пароль: " + password);
    }

    public static String generatePassword(int length) {
        String characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()";
        StringBuilder password = new StringBuilder();
