# ProcessingArrays
This program shows how to copy, compare, and search arrays.

public class processingArrays {
    public static void main(String[] arg) {
        int[] arr1 = {1, 2, 3, 4, 5, 6, 7};
        int[] arr2 = new int[arr1.length];

        //Copying an array
        for (int i = 0; i < arr2.length; i++) {
            arr2[i] = arr1[i];
            System.out.print(arr2[i] + " ");

        }
        //Comparing two arrays

        if (arr1.length != arr2.length) {
            System.out.println("The arrays are not equal.");
        }
        boolean equal = true;
        for (int i = 0; i < arr1.length; i++) {
            if (arr1[i] != arr2[i]) {
                equal = false;
            }


        }
        System.out.println("\n" + equal);
        //Searching for a value in an array
        int key = 5;
        for (int i = 0; i < arr1.length; i++) {
            if (arr1[i] == key) {
                System.out.println("Found at location " + i);
            }


        }
    }
}
