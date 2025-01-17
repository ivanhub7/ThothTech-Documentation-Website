---
title: "Creating a 2D Metroidvania in Splashkit: Introduction and Setup"
---

## Tutorial 1: Introduction and Setup

## Introduction

Welcome to the first tutorial in the "_Creating a 2D 'Metroidvania' Game Using Splashkit_" series.
In this tutorial, we'll embark on an exciting journey to create a 2D side-scrolling "Metroidvania"
game titled "Voidbound" using Splashkit. This series aims to introduce you to both the world of game
development and the powerful capabilities of Splashkit. By the end of this tutorial, you'll have a
clear understanding of the project's scope and the necessary setup steps.

## Splashkit Overview

Splashkit is a versatile software toolkit designed to simplify game development and programming. It
provides a wide range of function categories that empower developers to bring their creative ideas
to life. Some of the key function categories in Splashkit that we will explore in this series are:

1. **[Animations](https://splashkit.io/api/animations/)**: Allows for movement between cells in
   bitmaps and sprites, generating number sequences for drawing bitmaps.
1. **[Audio](https://splashkit.io/api/audio/)**: Utilise Splashkit Audio to load and play music and
   sound effects.
1. **[Camera](https://splashkit.io/api/camera/)**: Move a virtual camera around your game world
   using Splashkit camera functionality.
1. **[Color](https://splashkit.io/api/color/)**: Access utilities for creating, modifying, and
   converting colors, enhancing visual aesthetics.
1. **[Database](https://splashkit.io/api/database/)**: Create, query, and manipulate databases with
   Splashkit Database.
1. **[Graphics](https://splashkit.io/api/graphics/)**: Use Splashkit Text to draw text in various
   ways to graphic windows. Draw bitmaps and sprites using Splashkit Images.
1. **[Input](https://splashkit.io/api/input/)**: Handle user interaction and events like keypresses
   with Input functions.
1. **[JSON](https://splashkit.io/api/json/)**: Work with JSON objects through Splashkit JSON
   functionalities.
1. **[Physics](https://splashkit.io/api/physics/)**: Perform tests for collisions between bitmaps,
   sprites, and shapes using Splashkit Collisions. Use matrix and vector functions for 2D
   coordinates.
1. **[Resource Bundles](https://splashkit.io/api/resource-bundles/)**: Quickly load various
   resources in the `Resources` folder using Splashkit resource bundles.
1. **[Resources](https://splashkit.io/api/resources/)**: Locate resources in a project's `Resources`
   folder using Splashkit resource functions.
1. **[Sprites](https://splashkit.io/api/sprites/)**: Create movable and animated images with
   Splashkit Sprites.
1. **[Windows](https://splashkit.io/api/windows/)**: The Window Manager in Splashkit is used to
   create and manipulate graphics windows.

Click the category name to see an in-depth list of all the functions available in that category.
Don't worry if it all seems overwhelming. We're not going to use all these functions, and we will
explain the functions and how they work as they come up.

## Environment Setup

Before we dive into creating "Voidbound," let's ensure our development environment is ready:

### Installing Splashkit

To start creating games with Splashkit, you must first install it. Here's how:

1. **Visit the Splashkit Website**: Go to the
   [Splashkit website](https://splashkit.io/articles/installation/) and find the installation guide
   that matches your computer's platform.
1. **Follow the Guide**: The guide will provide you with step-by-step instructions. Make sure to
   follow them carefully. If there are any additional programs or libraries you need, the guide will
   let you know.

### Creating and Initialising Your New Project

Once Splashkit is installed, you're ready to create your first game project:

1. **Create a Project Folder**: Find a suitable location on your computer and create a new folder
   for your project. Let's call it "Voidbound."
1. **Using Splashkit Manager (SKM)**: Splashkit provides a tool called the Splashkit Manager (SKM)
   to help manage your projects. SKM commands follow a similar structure:
   `skm [command] [arguments]`.
1. **Create a New C++ Project**: Open your computer's terminal or command prompt and find to the
   "Voidbound" folder you just created. Run the command `skm new c++`. This will set up a new C++
   project for you.
1. **Generate Resource Folders**: Before diving into your project, there's one more thing to do. You
   can use SKM to generate the resource folders you will store game resources. Run the command
   `skm resources` in your project folder. This will create a "resources" folder where you can keep
   your game's assets.
1. **Open Your IDE**: Now, you're almost ready to start coding! In this tutorial series we are going
   to be using Visual Studio Code as our code editor, but you should be able to follow along in your
   editor of choice, so long as you set up the directories using the SKM and use SKM for compiling
   your code.

With these steps completed, you're all set up to begin working on your game project using Splashkit.
Happy coding!

## Conclusion and Next Steps

In this introductory tutorial, we've laid the foundation for our journey into creating a 2D
"Metroidvania" game titled "Voidbound" using Splashkit. We've gained a clear understanding of the
scope of this project and the powerful capabilities of Splashkit that we'll be utilising throughout
the series. Let's briefly recap what we've covered:

- **Splashkit Overview**: We explored the versatile features provided by Splashkit, ranging from
  animations, audio, and graphics to input handling, physics, and more.
- **Environment Setup**: We ensured that our development environment is ready by installing
  Splashkit and setting up our project using the Splashkit Manager (SKM).
- **Creating and Initialising Your New Project**: We created a new C++ project using SKM, generated
  resource folders, and prepared our code editor for coding.

Now that we've laid the groundwork, the next step is to delve into the exciting world of basic
drawing and graphics. In the upcoming tutorials, we'll learn how to create and manipulate graphics
windows, draw images, and bring our game world to life visually. By building upon what we've learned
here, we'll gradually shape "Voidbound" into a captivating gaming experience.

When you're ready, let's move on to the next tutorial: **Basic Drawing and Graphics**. Get ready to
unleash your creativity as we start coding and visualising our game's world. Happy coding and
designing your own "Voidbound" universe!
