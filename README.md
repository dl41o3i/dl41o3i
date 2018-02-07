# dl41o3i
字串平均數
public class Kata
{
  public static string AverageString(string str)
  {
    int v_ans = cut(str);
    return change2(v_ans);
  }
  public static int cut(string str)
  {
     int v_sum = 0; 
     int v_count = 0;
     string[] cut_arrary = str.Split(null);
     foreach (string i in cut_arrary)
     {
        v_sum = v_sum + change1(i);
        v_count = v_count + 1;
     }
     return (v_sum / v_count);   
  }
  public static int change1(string str)
  {
     int v_num = 0;
     switch (str)
     {
          case "one":
              v_num = 1;
              break;
          case "two":
              v_num = 2;
              break;
          case "three":
              v_num = 3;
              break;
          case "four":
              v_num = 4;
              break;
          case "five":
              v_num = 5;
              break;
          case "six":
              v_num = 6;
              break;
          case "seven":
              v_num = 7;
              break;
          case "eight":
              v_num = 8;
              break;                        
          case "nine":
              v_num = 9;
              break;
          case "zero":
              v_num = 0;
              break;    
          default:
              v_num = 99999; 
              break;
     }
     return (v_num);
  }
  public static string change2(int num)
  {
     string v_num = null;
     switch (num)
     {
          case 1:
              v_num = "one";
              break;
          case 2:
              v_num = "two";
              break;
          case 3:
              v_num = "three";
              break;
          case 4:
              v_num = "four";
              break;
          case 5:
              v_num = "five";
              break;
          case 6:
              v_num = "six";
              break;
          case 7:
              v_num = "seven";
              break;
          case 8:
              v_num = "eight";
              break;                        
          case 9:
              v_num = "nine";
              break;
          case 0:
              v_num = "zero";
              break;    
          default:
              v_num = "n/a"; 
              break;
     }
     return (v_num);
  }  
}
