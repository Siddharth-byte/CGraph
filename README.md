# CGraph
CGraph is a lightweight graph plotting library built in C using Raylib for rendering.
Overview
CGraph is a lightweight and simple-to-use graph plotting library written in C and powered by Raylib. It provides a clean API for visualizing data through common chart types:

Scatter Plot

Bar Graph

Histogram

Pie Chart

This project is ideal for anyone who needs basic data visualization in C applications with real-time rendering and minimal setup.

Features:

1.Supports Scatter, Bar, Histogram, and Pie charts

2.Custom Colors or automatic color assignment

3.Titles & Axis Labels for better readability

4.Lightweight and fast rendering using Raylib

5.Simple API for integration into your C projects

Tech Stack
Language: C

Graphics: Raylib

IDE: Visual Studio 2022 (or any C compiler)

Installation
Requirements
Raylib installed on your system.

C compiler (GCC/Clang) or Visual Studio.

Build Instructions
For Visual Studio:

Clone this repository:

bash
git clone https://github.com/your-username/CGraph.git
cd CGraph
Open Cgraph.sln in Visual Studio 2022.

Make sure Raylib include and lib directories are set:

Project → Properties → C/C++ → Additional Include Directories → raylib/include

Linker → Additional Library Directories → raylib/lib

Add raylib.lib to Linker → Input → Additional Dependencies.

Build and run.

For MinGW (Windows):
bash 
gcc main.c -o main.exe -lraylib -lopengl32 -lgdi32 -lwinmm
