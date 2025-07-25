public class Main
{
	public static void main(String[] args) {
		System.out.println("Hello World");
		int[] arr={1,1,2,3,3,4,4};
		int arrNumber=1;// index is strat from 1 if we give 0 so it cannot take first inputs
		for(int i=1;i<arr.length;i++){// if we star from 0 then it will give an error
		    if(arr[i]!=arr[i-1]){
		        arr[arrNumber]=arr[i];
		        arrNumber++;
		    }
		}
		 // Print the final array with unique elements
        System.out.print("Unique elements: ");
        for (int i = 0; i < arrNumber; i++) {
            System.out.print(arr[i] + " ");
        }
	}
}
