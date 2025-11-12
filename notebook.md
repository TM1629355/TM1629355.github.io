# My Coding Notebook

## Table of Contents
- [Flutter Notes](#flutter-notes)
  - [What is Flutter?](#what-is-flutter)
  - [Key Terms and Definitions](#key-terms-and-definitions)
  - [Layout and Design Widgets](layout-and-design-widgets)
  - [Definitions with Structures](#flutter-definitions-with-structures)
- [Code Definitions](#code-definitions)
-[Notebook Style Guide](#markdown-style-guide-for-coding-notebooks)

## Flutter Notes 

###  What is Flutter?
- A framework made by Google for building apps that work on the web, Android, and IOS-with one codebase.
- Uses the Dart programming language.


---

###  Key Terms and Definitions

| Term             | Definition                                      | Example / Notes                          |
|------------------|--------------------------------------------------|-------------------------------------------|
| Widget           | Basic building block of a Flutter app.           | Text, Image, Containter, Column           |
| MaterialApp      | The root of the app. Sets up routes and themes.  | Found in main.dart                        |
| Scaffold         | Provides basic visual layout-like a header, body, floating button| Each screen uses it       |
| StatelessWidget  | A widget that doesn't change                     | Most of the screen files                  |
| StatefulWidget   | A wdiget that can change over time               | Used in MyHomePage ()                     |
| Navigator        | Manages screen transitions                       | Navigator.pushNamed(context, '/page2);    |
| AppBar           | Top navigation bar                               | Title of each page appears here           |
| Column           | vertical layout                                  |                                           |
| Row              | horizontal layout                                |                                           |
| Container        | wraps content with padding, margin, or color     |                                           |
| Text             | displays text                                    |                                           |
| Image.network    | displays images from a URL                       |                                           |
| Padding          | adds space around a wdiget                       |                                           |
| Center           | centers its child                                |                                           |
| main()           | The function that runs the app                   | Found in main.dart                        |
| Named Routes     | Predefined paths to navigate between screens     | '/', '/page2', '/page3', etc.             |

---

### 🎨 Layout and Design Widgets
- How do you center a widget?
- How do you align something to the left or right?
- What widget adds space around content?

[Code Definitions](#code_definitions)

| Term | Definition | Base Structure / Syntax | Real Life Example | App Example |
|------|------------|--------------------------|-------------------|-------------|
| Algorithms | Define step by step processes to follow when completing a task or solving a problem | no syntax | Make a grilled cheese | Verify user |
| Sequencing | Define an order for when steps in an algorithm are completed | Follows 1, 2, 3 | which step comes first in making a grilled cheese | Get bread, add butter, add cheese |
| Variable | A named container used to store a value that may change. | `var x = 5;` |  | main.dart, String title: 'TSA Portfolio'|
| Constant | A fixed value that cannot change once set. | `const PI = 3.14;` |  | main.dart, const MyPortfolioApp ({super.key}); |
| Data Type | The kind of value a variable holds, like numbers or text. | `int`, `String`, `bool` |  | main.dart, bool, debugShowCheckModeBanner: false, |
| String | A sequence of characters used to represent words or text. | `"Hello World"` |  |  |
| Integer | Whole number values. | `int age = 16;` |  |  |
| Double | Number values with decimals. | `double age = 16.2;` |  |  |
| Boolean | A value that can be true or false. | `bool isLoggedIn = false;` |  |  |
| List | A collection of values in a specific order. | `List<String> names = [];` |  |  |
| Null | A special value that means “nothing.” | `String? name = null;` |  |  |
| Function | A reusable block of code that performs an action. | `void sayHi() { print("Hi"); }` |Turning on a car|  |
| Parameter | The information passed into a function to change how it works. | `greet(String name)` |  |  |
| Return | The result a function gives back. | `return total;` |  |  |
| Scope | Where a variable or function can be used. | (No set syntax — concept-based) |  |  |
| Class | Blueprint for creating objects with specific structure and behavior. | `class Dog {}` |  |  |
| Object | A specific version of a class. | `Dog myDog = Dog();` |  |  |
| Property | A variable that belongs to a class/object. | `String name;` |Limitations|  |
| Method | A function that belongs to a class. | `void bark() {}` |  |  |
| Constructor | A special function used to set up a class when it’s created. | `Dog(this.name);` |Knowing the design|  |
| Abstraction | Hiding the inner workings of code so users only interact with what they need. | (Concept — not specific code) |Keyboard and monitor|  |
| Override | Changing how a built-in or inherited function behaves. | `@override` |  |  |
| Void | A function that does not return a value. | `void printMessage() {}` |Missing a shot|  |
| Scanner |Creates a scanner object to take input from user|Scaner in = new Scanner(System.in);| | |
| impornt Scanner |Gives access to Scanner class, required at top|import java.util.Scanner;| | | 
| print line statement |prints what's in the parenthesis, adds line after|System.out.println(" ");| | |
| print statement |prints the content in the parenthesis|System.out.print(" ");| | |
| input nextLine |reads in a String from the user|input.nextLine();| | |
| input nextInt |reads in an int from the user|input.nextInt();| | |
| input nextDouble |reads in a double (decimal) from the user|input.nextDouble();| | |
| input nextBoolean |reads in a boolean (true/false) from the user|unput.nextBoolean();| | |
| Arithmetic operators |- + / % (modulus, returns the remainder from dividing)|    | | |
| Compound operators (applies to the variable) |+= -= *= /= %= ++ (adds 1)|    | | |
| Maximum int | The max value an int can hold: -2147483647 | Integer.MIN_VALUE | | |
| Minimum int | The minimum value an int can hold:-2147483648 | Integer.MIN_VALUE | | |
| intiger overflow | Integer.MAX_VALUE + 1 == MIN.VALUE, it wraps around | | |
| Intiger underflow | Integer.MIN_VALUE + 1 == MAX.VALUE, it wraps around | | |
| round-off error | an approx. of the actual value, result is around to the nearest value that fits within the available bits | | |
| Overloaded methold/function or constructor | Uses the same name, but has different parameters | Pizza(), Pizza(String toppings) 2 constructors, first is a default cheese pizza, 2nd has 1 topping | | |
| dot notation |Methods are called on objects using a dot after the object name | object.method(value); | | |
| Concatenate | To combine Strings with other Strings and/or variables | String greeting = "Hello" + "My name is" + name ". ";| | |


[Flutter Definitions](#flutter_definitions)
## Flutter Definitions

| Term | Definition and Description | Base Structure | Real Life Example | App Example |
|------|----------------------------|----------------|-------------------|-------------|
|main()| A function that runs when your app starts. It tells Flutter what app to show. | `void main() => runApp(MyApp());` |Opening a game|in main.dart, void main() => runApp(MyPortfolioApp()); |
|MaterialApp| The widget that sets up your whole app’s look and navigation. | `MaterialApp(...)` |  |main.dart, return MaterialApp(debugShowCheckModeBanner: false, tittle: 'TSA Portfolio', and more |
|Scaffold| A widget that gives you the basic layout: background, navigation bar, floating button, etc. | `Scaffold(...)` |A template|in showcase.dart, return Scaffold( body: Colum( mainAxisAlignment: MainAxisAlignment.start, children: [ |
|Column| A widget that holds and displays your content in a straight line from top to bottom. | `Column(...)` |Stacking things|in showcase.dart, body: Column( mainAxisAlignment: MainAxisAlignment.start, children: [ |
|Row| A widget that shows things side-by-side. | `Row(...)` |Putting things side by side|in InfoCard.dart, child: Row( |
|Container| A box that holds other widgets. You can add color, padding, borders, or size. | `Container(...)` |A canvas|in home.dart, Container(, widtch: 200, height: 200, decoration: BoxDecoration( |
|Text| A widget to display text on the screen. | `Text('Hello')` |  |in home.dart, const Text(, 'HI EVERYONE,\nWelcome to the' |
|Image.network| A widget to show an image using a link from the internet. | `Image.network('https://...')` |  |in home.dart, child: Image.network(, 'https://placedog.net/640/480?random' |
|ElevatedButton| A clickable button that floats above content. You choose what happens when it's clicked. | `ElevatedButton(onPressed: ..., child: ...)` |  |in home.dart, ElevatedButton(, onpressed: () => Navigator.pushNamed(context, '/background') |
|onPressed| The code that gets run when a button is tapped or something happens. | `onPressed: () => doSomething()` |  |in home.dart, ElevatedButton(, onpressed: () => Navigator.pushNamed(context, '/background') |
|StatelessWidget| A class that creates widgets that never change. Good for static screens. | `class HomeScreen extends StatelessWidget` |  |in home.dart, class HomeScreen extends StatelessWidget {, const HomeScreen({super.key}); |
|StatefulWidget| A class for widgets that can change while the app is running. | `class MyWidget extends StatefulWidget` |  |  |
|Navigator| Lets you move from one screen to another using route names. | `Navigator.pushNamed(context, '/about')` |  |in background.dart, ElevatedButton(, onPressed: () => Navigator.pushNamed(context, '/showcase'), child: const Text('Next'), |
|Padding| Makes space around a widget inside its container. | `Padding(padding: EdgeInsets.all(8.0), child: ...)` |Spacing around objects to look neater|in showcase.dart, Widget puppyImage(String url) {, return Padding(, padding: const EdgeInsets.all(4.0),|
|Center| Aligns content in the center of the screen or container. | `Center(child: ...)` |  |in home.dart, @override, Widget build(BuildContext context) {, return Scaffold(, body: Center( | 
|Wrap| Automatically puts widgets onto a new line when there's no space. | `Wrap(children: [...])` |going from one line to the next|in showcase.dart, Wrap(alignment: WrapAlignment.center, children: puppyUrls.map((url) => puppyImage(url)).toList()), |
|@override| This marks a method as one that’s replacing a method in a parent class. | `@override` |  |in InfoCard.dart, @override, Widget build(BuildContext context) { |
|build| The special function in every widget that describes what gets drawn on the screen. | `Widget build(BuildContext context) {...}` |  |in home.dart, @override, Widget build(BuildContext context) { |
|build| Required in every widget class to describe what to show. | `build` |  |in home.dart, @override, Widget build(BuildContext context) { |
|BuildContext| A variable that helps the widget know where it is and lets it communicate with the app. | `BuildContext context` |  |in home.dart, @override, Widget build(BuildContext context) { |
|super.key| A keyword used to pass a value to the parent widget. | `super.key` |emailing your teacher|in showcase.dart, class ShowcaseScreen extends StatelessWidget {, const ShowcaseScreen({super.key}); |
|const| A keyword that means the value won't change and is set once. | `const` |title|in InfoCard.dart, const InfoCard({, super.key, required this.imageUrl, required this.description, }); |


## Markdown Style Guide for Coding Notebooks

Follow this guide to keep your coding notebook **clear, consistent, and professional**.  
This ensures your notes are easy for you (and others) to read later.

---

## 🔹 Headings
**When to use:** Organize your notebook into sections (like days, topics, or projects).  
- `#` for the notebook title (use once at the top).  
- `##` for each day or major topic.  
- `###` for subsections (like "Notes", "Practice", "Reflections").  

✅ Example:


# My Coding Notebook
## Day 1
### Notes
### Practice

🔡 Text Formatting
When to use: Highlight important ideas or add emphasis.

Use bold for key terms or definitions.

Use italic for emphasis or side comments.

Use inline code for keywords, functions, or commands.

 

✅ Example:

**Class** = a blueprint for objects  
*Remember:* always test your code  
Use `System.out.println()` to print

 

💻 Code Blocks
When to use: Anytime you write multiple lines of code.

Inline code for short snippets.

Fenced code blocks with language for full examples.

✅ Example:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

🧾 Lists
When to use: Organize steps, notes, or key points.

Numbered lists for sequences or steps.

Bulleted lists for unordered ideas.

✅ Example:

1. Define the class
2. Write the main method
3. Test your program

Variables
- Loops
- Conditionals
 

✅ Checklists
When to use: Track progress on assignments or tasks.

✅ Example:

[x] Complete coding warm-up
- [ ] Finish project draft
- [ ] Reflect on learning

 

➡️ Blockquotes
When to use: Call out notes, reminders, or teacher comments.

✅ Example:

> 💡 Remember: Loops repeat code until a condition is false.

 

📊 Tables
When to use: Compare values, track progress, or organize data neatly.

✅ Example:

| Task        | Status   | Notes          |
|-------------|----------|----------------|
| Homework 1  | Done ✅  | Submitted      |
| Homework 2  | Pending  | Needs review   |

 

🔗 Links & Images
When to use: Add references, resources, or visuals.

✅ Example:

[Java Docs](https://docs.oracle.com/javase/8/docs/api/)  
![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

 

📂 Collapsible Sections
When to use: Hide solutions, extended notes, or extra details.

✅ Example:

<details>
  <summary>Click to reveal solution</summary>
  
System.out.println("Answer: 42");

</details>

 

📝 Footnotes
When to use: Add references or side notes without cluttering the page.

✅ Example:

This concept is related to object-oriented programming.[^1]

[^1]: See "Objects and Classes" in your textbook.

 

🎯 Style Rules
Consistency matters more than creativity

Always use headings to structure your notes.

Always use code blocks for multi-line code.

Clarity first

Bold key terms.

Use lists instead of long sentences when outlining steps.

Professional tone

Don’t mix casual notes with formal work in the same section.

Use blockquotes for reflections or teacher feedback.

Track your learning

Use checklists to mark what’s done.

Use collapsible sections if you want to hide answers until review time.

 

✅ Bottom Line:

Headings = Structure

Bold/Italic = Emphasis

Code blocks = Code

Lists = Steps/Ideas

Tables = Organization

Checklists = Progress

Blockquotes = Notes/Tips

Collapsible = Hide/Show detail

Keep it simple, consistent, and clear.
