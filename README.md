# CGraph
CGraph is a lightweight graph plotting library built in C using Raylib for rendering.
Overview
CGraph is a lightweight and simple-to-use graph plotting library written in C and powered by Raylib. It provides a clean API for visualizing data through common chart types:

Scatter Plot--void ScatterPlot(float[], float[], int, char[]);

Bar Graph--void BarGraph(float[], float[], int, char[]);

Histogram--void Histogram(const float* data, int count, int numBins, char color[]);

Pie Chart--void PieChart(const char** labels, float* values, int count, Color* colors);

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

Example: A simple scatter plot
// main.c
#include <stdio.h>
#include "Cgraph.h"

int main() {
    float x_data[] = { 1.0, 2.0, 3.0, 4.0, 5.0 };
    float y_data[] = { 5.5, 4.2, 7.8, 6.3, 9.1 };
    int data_count = 5;

    // Call library functions
    ScatterPlot(x_data, y_data, data_count, "BLUE");
    Print_Title("Sample Scatter Plot");
    Print_Axis_title("X-Axis", 'x');
    Print_Axis_title("Y-Axis", 'y');

    //  Render to handle the window loop and drawing
    Render();

    return 0;} 
    
Output:


![Scatter](https://github.com/user-attachments/assets/6a352cd6-201b-407f-90b8-75b3af0914d9)
