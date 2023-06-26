// java game to find actual name of 
//fruite

import java.util.*;
public class Main {
	public static int game(){
	    String [][]arr={{"apple","papel"},{"coconut","ocnoctu"}, {"pineapple","papipelne"},{"guava","augav"},{"mango","nogma"},{"papaya","yapapa"},{"brinjal","raljinb"} , {"tomato","motato"}};
	  int i=0;
	  int score=0;
	      while(i<8){
	        System.out.println("Guess this item  -:"+arr[i][1]);
	        Scanner input=new Scanner(System.in);
	        String val=input. nextLine();
	        if(val.equals(arr[i][0])){
	            System.out.println("Correct!");
	            score++;
	        }else{
	            System.out.println("actual word is  -"+arr[i][0]);
	        }i++;
	    }
	   
	  return score;  
	}
	public static void main(String[] args) {
		System.out.println("You will be given some name of fruits and vagitable in unarranged way");
		System.out.println("You have to gurss the actual name,and chack your overall score after completing the game");
		System.out.println("ARE YOU READY! Lets play");
	int score=	game();
	System.out.println("Your score is :"+score+"    out of 8");
	}
}