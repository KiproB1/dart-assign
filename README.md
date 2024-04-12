# dart-assign
Dart Utilities
// Task 1: Function to return the sum of two numbers
int sum(int a, int b) {
  return a + b;
}

// Task 2: Program to print numbers from 1 to 10 using a for loop
void printNumbers() {
  for (int i = 1; i <= 10; i++) {
    print(i);
  }
}

// Task 3: Program to use a switch statement to check different string values
void switchExample(String value) {
  switch (value) {
    case 'dart':
      print('Dart is awesome!');
      break;
    case 'java':
      print('Java is popular.');
      break;
    default:
      print('Language not recognized.');
  }
}

// Task 4: Program to print numbers from 20 to 10 using a while loop
void printNumbersDescending() {
  int i = 20;
  while (i >= 10) {
    print(i);
    i--;
  }
}

// Task 5: Program to check if a number is even or odd using if-else statement
void checkEvenOdd(int number) {
  if (number % 2 == 0) {
    print('$number is even.');
  } else {
    print('$number is odd.');
  }
}

// Task 6: Program to find the largest number in a list
int findLargestNumber(List<int> numbers) {
  if (numbers.isEmpty) return null;
  int largest = numbers[0];
  for (int i = 1; i < numbers.length; i++) {
    if (numbers[i] > largest) {
      largest = numbers[i];
    }
  }
  return largest;
}

// Task 7: Program to use try-catch block to catch an exception
void handleException() {
  try {
    // This line will throw an exception
    int result = 10 ~/ 0;
    print('Result: $result');
  } catch (e) {
    print('Error: $e');
  }
}

void main() {
  // Task 1: Testing the sum function
  print('Sum of 5 and 3: ${sum(5, 3)}');

  // Task 2: Printing numbers from 1 to 10
  print('Numbers from 1 to 10:');
  printNumbers();

  // Task 3: Switch example
  print('Switch Example:');
  switchExample('dart');
  switchExample('java');
  switchExample('python');

  // Task 4: Printing numbers from 20 to 10
  print('Numbers from 20 to 10:');
  printNumbersDescending();

  // Task 5: Checking if numbers are even or odd
  print('Checking even or odd:');
  checkEvenOdd(7);
  checkEvenOdd(10);

  // Task 6: Finding the largest number in a list
  print('Largest number in [5, 10, 3, 8, 12]: ${findLargestNumber([5, 10, 3, 8, 12])}');

  // Task 7: Handling exceptions
  print('Exception handling:');
  handleException();
}
