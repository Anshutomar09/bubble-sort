# bubble-sort

import java.util.*;
public class Main
{

  public static void sort (int arr[])
  {
    for (int i = 0; i < arr.length; i++)
      {
	System.out.print(arr[i]+ " ");
      }
  }

  public static void main (String args[])
  {

    int arr[] = { 7, 2, 9, 1,5 };

    for (int i = 0; i < arr.length ; i++)
      {
	for (int j = 0; j < arr.length - i ; j++)
	  {
	    if (arr[i] > arr[i + 1])
	      {
		int temp = arr[i];
		arr[i] = arr[i + 1];
		arr[i + 1] = temp;
	      }
	  }
      }
    sort (arr);

  }
}
