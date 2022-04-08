public class BubbleSort
{
        private int[] sortFunction(int[] unsortedArray){
            for(int i=0;i<unsortedArray.length-1; i++){
                for (int j=0;j<unsortedArray.length-i-1; j++){
                if (unsortedArray[j]> unsortedArray[j+1]){
                    int k=unsortedArray[j+1];
                    unsortedArray[j+1]=unsortedArray[j];
                    unsortedArray[j]=k;
                }     
                }     
          }
         return unsortedArray;
        }
    
    public static void main(String args[]) {
        BubbleSort bubbleSort=new BubbleSort();
        int[] unsortedArr={1,7,3,2,5};
        int [] sortedArray=bubbleSort.sortFunction(unsortedArr);
             for(int i=0;i<sortedArray.length; i++){
                 System.out.println(sortedArray[i]);
             }
    }

}
