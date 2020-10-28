     
     
     
     import java.util.Scanner; 
      public class JavaIdentificationCode {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.println("Name");
        String name = input.nextLine();
        System.out.println("Location");
        String location = input.nextLine();
        System.out.println("Date of birth");
        String dob = input.nextLine();
        System.out.println("gender");
        String gender = input.nextLine();

        // substring
        // indexOf
        // lastIndexOf
        // length
        // concat
        // toUpperCase

        //First Name
        
        String firstNameLetter= name.substring(0, 1);
        int space = name.indexOf(" ");






        //Last Name
        
        //int indexOfSpace = "name".indexOf(" "); // 6
        //System.out.println("The character is: " + "name".substring(indexOfSpace + 1, indexOfSpace + 2));
        String lastNameLetter = name.substring(space + 1, space + 2);





        //Zipcode
        
        int zipCodeSpace = location.length();
        //System.out.println("The last digit of zip: " + location.substring(zipCodeSpace - 3)); 
        String lastZip = location.substring(zipCodeSpace - 3);
        //String location = zipCodeSpace.length(zipCodeSpace - 3);
        




        //DOB
        
        int dateOfBirth = dob.length();
        //System.out.println("Last digit of dob: " + dob.substring(dateOfBirth - 2));
        String year = dob.substring(dateOfBirth - 2);






        //Gender 
        
        String firstLetterGender = gender.substring(0,1);
        String firstLetterGenderUpper = firstLetterGender.toUpperCase();






        //State
        
        int stateComma = location.lastIndexOf(", ");
        String state = location.substring(stateComma + 2, stateComma + 4);
        




        
        //Identification 
        System.out.println("Identification code: " + firstNameLetter + lastNameLetter + "-" + lastZip + year + "-" + firstLetterGenderUpper + state);
