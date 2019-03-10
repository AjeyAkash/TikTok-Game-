# TikTok-Game-
TikTok Gaame is in java .
import java.util.Scanner;

class TikTok
       {
             public static void main(String args[])
	   {
	        Scanner in =new Scanner(System.in);
                        System.out.println("\t WELCOME TO TIC TAC TOE GAME");
                        System.out.println("Enter The Players Name :");
                        String n1 =in.nextLine();
                        String n2 =in.nextLine();
                        char a1[][]= new char[3][3] ;
                        char a2='0';    
                        char a;
                        
                          for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {    
        		            a1[i][j]=++a2;
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                                                         
                        
                           for(int k=0;k<10;k++)
                              { 
                                      
                                       if(k>=5)
                                        {
                                             if((a1[0][0]=='X' && a1[0][1]=='X' && a1[0][2]=='X')||(a1[1][0]=='X' && a1[1][1]=='X' && a1[1][2]=='X')||(a1[2][0]=='X' && a1[2][1]=='X' && a1[2][2]=='X')||(a1[0][0]=='X' && a1[1][0]=='X' && a1[2][0]=='X')||(a1[0][1]=='X' && a1[1][1]=='X' && a1[2][1]=='X')||(a1[0][2]=='X' && a1[1][2]=='X' && a1[2][2]=='X')||(a1[0][0]=='X' && a1[1][1]=='X' && a1[2][2]=='X')||(a1[0][2]=='X' && a1[1][1]=='X' && a1[2][0]=='X'))
                                                   {
                                                     System.out.println(n2+" Wins Congratulations");
                                                     break;
			   }
                                             else if((a1[0][0]=='O' && a1[0][1]=='O' && a1[0][2]=='O')||(a1[1][0]=='O' && a1[1][1]=='O' && a1[1][2]=='O')||(a1[2][0]=='O' && a1[2][1]=='O' && a1[2][2]=='O')||(a1[0][0]=='O' && a1[1][0]=='O' && a1[2][0]=='O')||(a1[0][1]=='O' && a1[1][1]=='O' && a1[2][1]=='O')||(a1[0][2]=='O' && a1[1][2]=='O' && a1[2][2]=='O')||(a1[0][0]=='O' && a1[1][1]=='O' && a1[2][2]=='O')||(a1[0][2]=='O' && a1[1][1]=='O' && a1[2][0]=='O'))
                                                   {
                                                     System.out.println(n1+ " Wins Congratulation");
                                                     break;
                                                   }
                                          
                                                
                                          }   
                                   
                                if(k<9){
                                 if(k%2==0)
                                       {
                                            System.out.println("Your Chance "+ n1);
                                            a ='O';    
                                       }
                                   else
                                       {    
                                             System.out.println("Your Chance "+n2);
                                            a ='X';
                                       }
                           
                            int b = in.nextInt();
                           
                           switch(b)
                           {  
                           case 1:
                            if(a1[0][0]=='X'||a1[0][0]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                           a1[0][0] =a;
                              for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {   
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                           break;
                            
	            case 2:
                            if(a1[0][1] =='X'||a1[0][1]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[0][1] =a;
                               for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {    
        		            
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            break;

	            case 3:
                             if(a1[0][2]=='X'||a1[0][2]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[0][2] =a;
                             for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {    
        		            
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            break;

	            case 4:
                             if(a1[1][0]=='X'||a1[1][0]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[1][0] =a;
                               for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {    
        		            
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                           break; 

	            case 5:
                             if(a1[1][1]=='X'||a1[1][1]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[1][1] =a;
                            for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {    
        		           
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            break;
                             
	            case 6:
                             if(a1[1][2]=='X'||a1[1][2]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[1][2]=a;
                              for(int i=0;i<3;i++)
	             {
                                  for(int j=0;j<3;j++)
                                       {    
        		           
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            
                            break;
                            
	            case 7:
                             if(a1[2][0]=='X'||a1[2][0]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[2][0]=a;
                               for(int i=0;i<3;i++)
	                  {
                                  for(int j=0;j<3;j++)
                                       {    
        		            
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            break;
                            
	            case 8:
                             if(a1[2][1]=='X'||a1[2][1]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                            a1[2][1] =a;
                               for(int i=0;i<3;i++)
	                  {
                                  for(int j=0;j<3;j++)
                                       {    
        		            
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            break;
                           
	            case 9:
                             if(a1[2][2]=='X'||a1[2][2]=='O')
                            { 
                               System.out.println("ERROR HAS BEEN OCCURED : PLEASE TRY AGAIN");
                               k--;
                               continue;
                            }
                               a1[2][2] =a;
                               for(int i=0;i<3;i++)
	                  {
                                  for(int j=0;j<3;j++)
                                       {    
        		           
                                            System.out.print("\t" + a1[i][j]);
                                        }
                                  System.out.println();
                             }
                            break; 
                            
                            default:
                            System.out.println("Wrong Choice");
                            k--;
                                                   
                    }     }
                            
                            if(k==9)
                            System.out.println("Match Drawn");
            }
      }
      
}
