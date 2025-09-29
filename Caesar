public class Caesar {
    public static void main(String[] args) {
        
        if (args.length < 2) {
            System.out.println("Please provide a shift key and at least one message (<K> <Message_1> ... <Message_N>).");
            System.exit(-1);
        }
        
        int K = Integer.parseInt(args[0]); // Variable for the shift key
        
        for (int i = 1; i < args.length; i++) { // Loop through all messages starting from the second argument
            String message = args[i]; // message to be encrypted
            String encryptedMessage = ""; // empty string to store the encrypted message
            
            for (char letter : message.toCharArray()) { // for-each loop iterates through each character of the message
                
                char base = 0;
                
                if (letter >= 'A' && letter <= 'Z') { // check if the character is an uppercase letter
                    base = 'A';
                }
                
                if (letter >= 'a' && letter <= 'z') { // check if the character is a lowercase letter
                    base = 'a';
                }
                
                if (letter >= 'A' && letter <= 'Z' || letter >= 'a' && letter <= 'z') { 
                    // if the character is a valid letter (uppercase or lowercase),
                    // apply Caesar shift. Non-letter characters remain unchanged.
                    letter = (char) ((letter - base + K + 26) % 26 + base); 
                }
                
                encryptedMessage += letter; // add the encrypted character to the result string
            }
            
            System.out.println(encryptedMessage); // print the encrypted message
        }
    }
}
