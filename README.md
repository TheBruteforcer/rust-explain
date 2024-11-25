
basics 

golang 
memory preserved 





```rust
use std::io;

fn main(){
	println!("Hello, Omar !");
}
```

```bash
Hello, Omar !
```



```rust

fn main(){
	let x = 3;
	let y = 7;
	let name = "Omar" ; // String
	let degree = "A"; // char
	
}

```


*Data Types*
 - i32 , i64, i128

 - str, char "Omar", 'A'
 - bool
 - f






```rust
// Import necessary libraries
use std::collections::HashMap;
use std::io;

cout 
cin

struct Person {
    name: String,
    age: u8,
}
impl Person {
	// display(self) . New person
	// impl , self Person 
	// & 0X1104995 var 
    fn display(&self) {
        println!("Name: {}, Age: {}", self.name, self.age);
    }

    fn new(name: String, age: u8) -> Self {
        Person { name, age }
        println!("Created Person , {}, {}", ...)
    }
}

Person.display()

x = Person < 
&x.display()

Person 
 - impl
  - display(&self)












struct vec{
....
}

let v = vec{...}

&v 















// Function to demonstrate vectors
fn demonstrate_vectors() {
    // Create a vector of integers
    let mut numbers = vec![1, 2, 3, 4, 5];
    println!("Initial vector: {:?}", numbers); [1,2,3] 1 2 3 

    // Add elements to the vector
    numbers.push(6); // 1,2,3 // 1,2,3,4
    numbers.push(7);
    println!("After adding elements: {:?}", numbers);

    // Remove an element
    numbers.pop(); // 1,2,3 // 1,2 
    println!("After removing an element: {:?}", numbers);

	println!(numbers.get(0));
    // Access elements
	// [] print(vec[0])
    if let Some(first) = numbers.get(0) {
        println!("First element: {}", first);
    }
}

// Function to demonstrate arrays
fn demonstrate_arrays() {
    // Define an array of strings
    let fruits = ["Apple", "Banana", "Cherry", "Date"]; 4
    println!("Fruits array: {:?}", fruits);

    // Access array elements by index
    println!("First fruit: {}", fruits[0]);
    println!("Last fruit: {}", fruits[fruits.len() - 1]);

    // Iterate over the array
    ARR
     - impl
      - iter(&self) 
    for fruit in fruits.iter() {
		["Me", "You"]
		0 Me
		1 You
        println!("Fruit: {}", fruit);
    }
}


for (new var) in (arr - present).iter(){

}

[1, 2, 3]

for e in arr.iter(){
print(e)
}

 > 1 > print > 1
 > 2
e>   3














// Function to demonstrate hash maps
fn demonstrate_hash_maps() {
    // Create a HashMap
    let mut scores = HashMap::new();

    // Insert key-value pairs
    scores.insert("Alice", 10); insert(key : any, value : any)
    scores.insert("Bob", 20);
    scores.insert("Charlie", 30); {"Alice" : 10}

    println!("Initial HashMap: {:?}", scores); // {"Alice" : 10}

    // Access a value
    if let Some(score) = scores.get("Alice") {
        println!("Alice's score: {}", score);
    }

    // Remove a key-value pair
    scores.remove("Bob");
    println!("After removing Bob: {:?}", scores); // {Alice : 10, Charlie : 30}

    // Iterate over key-value pairs
    for (name, score) in &scores {
        println!("{}: {}", name, score);
    }

for loop
(e, z)
loop 1
e, z > Alice   10> e=Alice , z = 10
Bob     20
Charlie 30




}


String
 - impl 
  - constructor > ::new
  - trim
  - to_string (Struct to String)
  - clear

let mut input = String::new()

&input < val

more variable > more ram

input.clear()



io::stdin()
	.read_line(...)
	.expect(...)\

fn play
   ......
play;
	.expect("Failed");

// Main function: Entry point of the program
fn main() {
    let mut input = String::new(); 1 , "Hello" + " Omar" =  "Hello Omar"
    1 + "Hello" = ??
    println!("Enter your name:");
    io::stdin()                 Enter your name : 
        .read_line(&mut input)
        .expect("Failed to read input"); "true"
    let name = input.trim().to_string();

    println!("Enter your age:"); 

	Console > Input > 20 > Code > "20" > Parse > 20 < Code

    input.clear();
    io::stdin()
        .read_line(&mut input)
        .expect("Failed to read input");

	Age > 20 > Operation (2024 - age) > 2004

    let age: u8 = input
        .trim()
        .parse()
        .expect("Please enter a valid number");

	Variable = ...(struct) > type > struct

    let person = Person::new(name.clone(), age);
    person.display();

    // Use an if-else statement
    if age >= 18 {
        println!("{} is an adult.", name);
    } else {
        println!("{} is not an adult.", name);
    }

    println!("\n--- Demonstrating Vectors ---");
    demonstrate_vectors();

    println!("\n--- Demonstrating Arrays ---");
    demonstrate_arrays();

    println!("\n--- Demonstrating Hash Maps ---");
    demonstrate_hash_maps();
}

```




### 

![‪R Vectors - GeeksforGeeks‬‏](data:image/jpeg;base64,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)







](https://www.google.com/imgres?q=vectors%20programming&imgurl=https%3A%2F%2Fmedia.geeksforgeeks.org%2Fwp-content%2Fuploads%2F20200409134016%2FVectors-in-R.jpg&imgrefurl=https%3A%2F%2Fwww.geeksforgeeks.org%2Fr-vector%2F&docid=kam4rq10VV_QLM&tbnid=GRs8f8d4Q6ygsM&vet=12ahUKEwi_qd79rviJAxV6Q6QEHb32FkwQM3oECBcQAA..i&w=622&h=282&hcb=2&ved=2ahUKEwi_qd79rviJAxV6Q6QEHb32FkwQM3oECBcQAA)











































