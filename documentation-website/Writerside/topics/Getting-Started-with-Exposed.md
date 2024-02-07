# Getting Started with Exposed

Welcome to the `Getting Started with Exposed` tutorial. In this tutorial we are going to create a simple application
that will demonstrate how to use Exposed to interact with a database.

## Prerequisites

Before you start, you need to have a basic understanding of Kotlin programming language. If you're new to Kotlin,
please check [Learning Materials](https://kotlinlang.org/docs/learning-materials-overview.html) section on the Kotlin
website.

You also need to have the following installed on your machine:

- JDK8 (Java Development Kit) installed on your machine.

On the screenshots, we are using IntelliJ IDEA as our IDE. If you don't have it, you can download
it free from the official [JetBrains website](https://www.jetbrains.com/idea/download/). You can also use any other IDE.

## Setting up the project

In this tutorial we're going to build a TODO list application. We'll start by creating a new Kotlin Gradle project
using.
To create a new Kotlin project it's easy to use IDEA's New Project wizard.

![1._Exposed_Create_TODO_app.png](1._Exposed_Create_TODO_app.png)

If you don't have, you can download the new project template [here]().

After opening the project, your project tree will look like this:
![2. Project Tree.png](2._Project_Tree.png)

## Adding Exposed to the project

Before we start working with Exposed, we need to add the dependency to our project. For this sample we're going to use
[H2 database](https://www.h2database.com/html/main.html).

To add Exposed to the project, open the `build.gradle.kts` file and add the following dependencies to the `dependencies` block:

```kotlin
val exposedVersion = "0.47.0"

dependencies {
    implementation("org.jetbrains.exposed:exposed-core:$exposedVersion")
    implementation("org.jetbrains.exposed:exposed-jdbc:$exposedVersion")
    
    // ...
}
```

## Define Schema Tables

## Connecting to the Database