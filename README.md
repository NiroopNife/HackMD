# HackMD

void main() {
	
  checkAge('Nife', 30); //Function to check how many more years to be 100 year old
  
  evenOrOdd(10); //Function to check if the given Number is Odd or Even
  
  lessThan5([1, 2, 3, 4, 5, 6, 7, 8, 9]); //Function to create a new list where in the array shold contain numbers less than 5 only
  
  compare2Lists([1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89], [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13]); //A new list consisting of same values in both lists
  
  palindromeString('abcbp'); //Check if the given string is a palindrome or not
  
  palindromeNumber(120); //Check if the given number is palindrome or not
  
  evenList([1, 4, 9, 16, 25, 36, 49, 64, 81, 100]); //Create a new list conisiting of only even numbers
  
}

Even List -->
```
evenList(List exampleList) {
  print([for (var i in exampleList) if (i % 2 == 0) i]);
}
```

Palindrome Number -->
```
palindromeNumber(int number) {
  int reminder, sum = 0, temp;
  temp = number;
  while(number>0){
    reminder = number % 10;  //get remainder
    sum = (sum*10)+reminder;
    number = number~/10;
  }

  sum == temp ? print("Palindrome number") : print("Not a palindrome number");
}
```
Palindrome String -->
```
palindromeString(String word) {
  String reverseWord = word.split('').reversed.join('');
  reverseWord == word ? print("Palindrome String") : print("Not a palinrome");
}
```
Comparision between 2 Lists -->
```
compare2Lists(List l1, List l2) => l1
    .toSet()
    .where((x) => l2.toSet().contains(x))
    .toList();
```

Print only items less than 5 -->
```
lessThan5(List integers) =>
  print([for (var i in integers) if (i < 5) i]);
```

Check the number is even or odd -->
```
evenOrOdd(int num) =>
  (num > 0 && num % 2 == 0) ? print("Even") : print("Odd");
```

Check age to become 100 year old -->
```
checkAge(String name, int age) => 
  print('$name, you have ${100 - age} more years to be 100 years old');
```
