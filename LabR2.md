# Lab Report 2
## Part 2
The following block of code should return a new array with all of the elements in the input array in reversed order.
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
Insted of revesing the order the array would be full of zeros.
!Image()

To fix this code I switched which array was being copied and returned the new array that was produced.
Here is the function code:
```
  static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
  ```
