# Data Structure Analysis API

A beginner-friendly **Data Structures and Algorithms (DSA)** project built using **C#, .NET, and ASP.NET Core Web API**.

This project demonstrates fundamental data structure concepts through practical API endpoints. The code is organized using **Controllers, Models, and Services** to keep the project clean and easy to understand.

## 📚 Topics Covered

* Arrays
* Array Traversal
* Array Insertion
* Array Deletion
* Array Update
* Linear Search
* Reverse Array
* Remove Duplicate Elements
* Find Maximum and Minimum
* Factorial
* Multiplication
* Time Complexity
* Big-O Analysis
* Student Management
* CRUD Operations
* Object-Oriented Programming (OOP)
* ASP.NET Core Web API

## 🗂️ Project Structure

```text
DataStructureAnalysis-main/
│
├── Controllers/
│   ├── ArrayController.cs
│   ├── ComplexityController.cs
│   ├── FactorialController.cs
│   ├── MultiplicationController.cs
│   ├── ReflectionController.cs
│   ├── SetupController.cs
│   └── StudentsController.cs
│
├── Models/
│   └── Dtos.cs
│
├── Services/
│   ├── ArrayOperations.cs
│   ├── BigOAnalysisService.cs
│   ├── FactorialService.cs
│   ├── MultiplicationService.cs
│   ├── StudentManager.cs
│   └── TimingService.cs
│
├── Notes/
│   ├── Lab0-Introduction.docx
│   └── Lab1-Array.docx
│
├── Properties/
│   └── launchSettings.json
│
├── Program.cs
├── DSALabsApi.csproj
├── appsettings.json
└── README.md
```

## 🔢 Array Operations

The `ArrayOperations` service contains the main array logic.

### Task 01 – Basic Array Operations

* Traverse the array
* Insert element at the end
* Insert element at the beginning

### Task 02 – Position-Based Operations

* Insert element at a specific position
* Delete element from a specific position
* Delete element from the end

### Task 03 – Update and Search

* Update an element at a specific position
* Linear Search
* Search for all occurrences of an element

### Task 04 – Delete From Beginning

* Delete the first element of the array
* Shift remaining elements to the left

## ✨ Additional Array Features

### Reverse Array

Reverses the order of elements in an array.

Example:

```text
Input:  [10, 20, 30, 40]
Output: [40, 30, 20, 10]
```

### Remove Duplicates

Removes duplicate values and returns only unique elements.

Example:

```text
Input:  [10, 20, 20, 30, 30, 40]
Output: [10, 20, 30, 40]
```

### Find Maximum and Minimum

Finds the largest and smallest values in an array.

Example:

```text
Input: [10, 50, 20, 5, 30]

Maximum: 50
Minimum: 5
```

## ⏱️ Time Complexity

Some important array operation complexities demonstrated in this project:

| Operation             | Time Complexity |
| --------------------- | --------------- |
| Access by index       | O(1)            |
| Update by index       | O(1)            |
| Insert at end         | O(1)            |
| Delete from end       | O(1)            |
| Insert at beginning   | O(n)            |
| Delete from beginning | O(n)            |
| Insert at position    | O(n)            |
| Delete at position    | O(n)            |
| Linear Search         | O(n)            |
| Reverse Array         | O(n)            |
| Remove Duplicates     | O(n) average    |
| Find Maximum/Minimum  | O(n)            |

## 🛠️ Technologies Used

* C#
* .NET 9
* ASP.NET Core Web API
* Swagger / OpenAPI
* Visual Studio / VS Code
* Git
* GitHub

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <repository-url>
```

### 2. Open the project folder

```bash
cd DataStructureAnalysis-main
```

### 3. Restore dependencies

```bash
dotnet restore
```

### 4. Run the application

```bash
dotnet run
```

### 5. Open Swagger

After running the application, open the Swagger URL shown in the terminal.

Swagger can be used to test the API endpoints directly from the browser.

## 🧩 Project Architecture

The project follows a simple layered structure:

**Controllers**
Handle HTTP requests and return API responses.

**Services**
Contain the main DSA algorithms and business logic.

**Models**
Contain DTOs and request/response classes used by the API.

**Program.cs**
Configures controllers, Swagger, dependency injection, and application services.

## 💉 Dependency Injection

Services are registered in `Program.cs`.

Example:

```csharp
builder.Services.AddSingleton<ArrayOperations>(
    sp => new ArrayOperations(15));

builder.Services.AddSingleton<StudentManager>();
builder.Services.AddSingleton<FactorialService>();
builder.Services.AddSingleton<MultiplicationService>();
builder.Services.AddSingleton<TimingService>();
builder.Services.AddSingleton<BigOAnalysisService>();
```

`ArrayOperations` is registered as a **Singleton**, allowing its array state to persist between API requests while the application is running.

## 🎯 Learning Objectives

This project helps students learn how to:

* Understand arrays and their operations
* Implement DSA concepts using C#
* Understand time complexity
* Practice Big-O analysis
* Create REST API endpoints
* Use Controllers, Models, and Services
* Apply Object-Oriented Programming concepts
* Use Dependency Injection
* Test APIs using Swagger
* Organize a .NET project properly

## 🔮 Future Improvements

More data structures and algorithms can be added, such as:

* Linked Lists
* Stacks
* Queues
* Hash Tables
* Trees
* Binary Search Trees
* Graphs
* Recursion
* Binary Search
* Bubble Sort
* Selection Sort
* Insertion Sort
* Merge Sort
* Quick Sort

## 👨‍💻 Author

**Khaleel Afzal**

This project is created for learning, practicing, and understanding **Data Structures and Algorithms using C# and ASP.NET Core**.

## 📄 License

This project currently does not specify a license.
