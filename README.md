# HackMD

* Check age to become 100 year old -->

Create a program that asks the user to enter their name and their age. Print out a message that tells how many years they have to be 100 years old.
```
checkAge(String name, int age) => 
  print('$name, you have ${100 - age} more years to be 100 years old');
```

* Check the number is even or odd -->

Ask the user for a number. Depending on whether the number is even or odd, print out an appropriate message to the user.
```
evenOrOdd(int num) =>
  (num > 0 && num % 2 == 0) ? print("Even") : print("Odd");
```

* Print only items less than 5 -->

Take a list and write a program that prints out all the elements of the list that are less than 5.
```
lessThan5(List integers) =>
  print([for (var i in integers) if (i < 5) i]);
```

* Palindrome String -->

Ask the user for a string and print out whether this string is a palindrome or not.
```
palindromeString(String word) {
  String reverseWord = word.split('').reversed.join('');
  reverseWord == word ? print("Palindrome String") : print("Not a palinrome");
}
```

* Palindrome Number -->

Ask the user for a number and print out whether this number is a palindrome or not.
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

* Unique List -->
```
uniqueList(List someList) => someList.toSet().toList());
```

* Reverse sentence -->
```
reverseSentence(String sentence) => sentence.split(" ").reversed.toList().join(" "));
```

* Largest in a List -->
```
largestInList(List numbers) {
  numbers.sort();
  print(numbers.last);
}
```

* Largest in given -->
```
largest(int a, int b, int c) {
  var max;
  a > b ? max = a : max = b;
  c > max ? max = c : max = max;
  print(max);
}
```

* First and Last elements of a List in a New List -->
```
firstAndLastList(List someList) {
  List anotherList = [someList.first, someList.last];
  print("Another List $anotherList");
}
```

* Prime Number -->
```
primeNumber(int number) {
  List<int> a = [
    for (var i = 1; i <= number; i++)
    if (number % i == 0) i
 ];
  a.length == 2 ? print("The chosen number is a prime")
      : print("The chosen number is not a prime");
}
```

* Even List -->
```
evenList(List exampleList) {
  print([for (var i in exampleList) if (i % 2 == 0) i]);
}
```

* Comparision between 2 Lists -->
```
compare2Lists(List l1, List l2) => l1
    .toSet()
    .where((x) => l2.toSet().contains(x))
    .toList();
```


