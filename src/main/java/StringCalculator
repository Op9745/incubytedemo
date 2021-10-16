package calculator;

class StringCalculator {

    public int add(String input) {
        //empty string should return zero
        if(input.length()==0){
            return 0;
        }
        //single no string returns no as int 
        else if(input.length()==1)
        {
            return Integer.parseInt(input);
        }
        // return sum as int
        else if(input.length() == 2)
        {
            String[] st=input.split(",");
            return Integer.parseInt(st[0]) + Integer.parseInt(st[1]);
        }
        // new line handling and return sum
        else if(input.contains("\n") && input.contains(","))
        {
            int result=0;
            input=input.replace("\n", "");
            String[] st=input.split(",");
            for(int in=0;in<st.length;in++){
                result= result + Integer.parseInt(st[in]);
            }
            return result;
        }
        //multiple delimiter handling and return sum
        else if(input.contains("//") && input.contains("\n"))
        {
            int result=0;
            input= input.replace("//","0");
            input= input.replace("\n", "");

            String[] st= input.split(";");
            for(int in=0;in<st.length;in++){
                result= result + Integer.parseInt(st[in]);
            }
            return result;
        }
        //multiple nos. and return sum
        else{
            int result=0;

            String[] st= input.split(",");
            for(int in=0; in<st.length;in++){
                result=result + Integer.parseInt(st[in]);
            }
            return result;
        }   
    }
}
