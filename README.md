# problem-solving---arrows-to-burst-all-the-ballons

Find the minimum number of arrow to burst ballons.
Given a ets osfs bsallons each repreented by a range start , end find the minimum number of arrows required to burst all the ballons. An arrow can burst multiple ballons if they overlap.

import java.util.*;
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[][] ballons = {{1,6},{2,8},{7,12},{10,16}};
        int arrows = 1;
        int current =  ballons[0][1];
        for(int i=0;i<n;i++){
            if(ballons[i][0]>current){
                arrows++;
                current = ballons[i][1];
            System.out.println(arrows);
            }
        }
    }
}
