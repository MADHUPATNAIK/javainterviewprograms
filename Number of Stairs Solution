import java.io.*;
import java.util.*;

class StairsSolution{
  public static void main(String[] args) throws IOException{
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
        
        int totalNumberOfSteps = Integer.parseInt(br.readLine());
        
        int stepsAtOnceTaken = Integer.parseInt(br.readLine());
        
        int[] numberOfStepsArray = new int[stepsAtOnceTaken];
        
        StringTokenizer st = new StringTokenizer(br.readLine());
        for(int i=0; i<stepsAtOnceTaken; i++){
            numberOfStepsArray[i] = Integer.parseInt(st.nextToken());
        }
        
        int countWays = calculateNumberOfSteps(totalNumberOfSteps, numberOfStepsArray);
        System.out.println(countWays);
    }
    
    public static int calculateNumberOfSteps(int n, int[] stepsArr){
        if(n == 0) return 1;
        else if (n<0) return 0;
        else{
            int x = 0;
            for(int i=0; i<stepsArr.length; i++)
                x+=calculateNumberOfSteps(n-stepsArr[i], stepsArr);
            return x;
        }
    }
}
