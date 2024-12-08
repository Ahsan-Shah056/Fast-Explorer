# Fast Explorer: City Navigation and Travel Cost System

Welcome to **Fast Explorer**, a comprehensive system that combines geographical exploration, shortest path calculations, and travel cost estimations in an interactive and intuitive application. This system provides users with insights into cities across Pakistan and helps calculate optimal travel routes and costs based on passenger type and vehicle preferences.

---

## Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [System Design](#system-design)
4. [Getting Started](#getting-started)
5. [User Guide](#user-guide)
6. [Technology Stack](#technology-stack)
7. [Future Enhancements](#future-enhancements)

---

## Overview

**Fast Explorer** is designed to:

- Display cities and their geographical coordinates.
- Show neighboring cities and their connections.
- Calculate the shortest path between two cities using **Dijkstra’s algorithm**.
- Estimate travel costs based on passenger type (e.g., student, adult, elderly) and vehicle choice (e.g., mini, standard, luxury).

This system leverages advanced algorithms, data structures, and user interaction to provide a seamless and educational experience for exploring Pakistan’s geography and travel options.

---

## Features

### 1. City Information

- View cities and their geographical coordinates (latitude and longitude).
- Understand city connections and neighboring cities.

### 2. Shortest Path Calculation

- Calculate the shortest path between two cities using **Dijkstra’s algorithm**.
- View the path step-by-step with cumulative distances.

### 3. Travel Cost Estimation

- Calculate travel costs based on:
  - **Passenger category**:
    - **Student**: 50% discount.
    - **Elderly**: 20% discount.
    - **Adult**: Full price.
  - **Vehicle type**:
    - **Mini**: Rs. 20 per km.
    - **Standard**: Rs. 50 per km.
    - **Luxury**: Rs. 20 per km with additional discounts for students and elderly.

### 4. User-Friendly Interface

- Interactive menu-driven interface for seamless navigation.
- Visual feedback for user input and results.

---

## System Design

### Core Components

1. **Graph Representation**:
   - Cities are represented as vertices in a graph.
   - Connections between cities are represented as edges.

2. **Shortest Path Algorithm**:
   - **Dijkstra’s algorithm** calculates the shortest path and distance between two cities.

3. **Passenger Classes**:
   - Inheritance and polymorphism provide dynamic cost calculations based on passenger type.

4. **Vehicle Classes**:
   - Modular design allows dynamic cost-per-kilometer calculations based on vehicle choice.

5. **Geographical Coordinates**:
   - The **Haversine formula** calculates the distance between cities using latitude and longitude.

---

## Getting Started

### Requirements

- A **C++ compiler** (e.g., GCC, Clang).
- A terminal or IDE for running the program.

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-repo/fast-explorer.git
    ```

2. Navigate to the project directory:

    ```bash
    cd fast-explorer
    ```

3. Compile the program:

    ```bash
    g++ fast_explorer.cpp -o fast_explorer
    ```

4. Run the executable:

    ```bash
    ./fast_explorer
    ```

---

## User Guide

### Main Menu

After launching the program, you will see the following menu:

1. **Display Cities**  
   - Shows all cities with their geographical coordinates.

2. **Display Neighboring Cities**  
   - Shows each city with its neighboring cities.

3. **Calculate Path and Costs**  
   - Enter your source and destination cities.
   - Choose your passenger type and vehicle type.
   - View the shortest path, distance, and travel cost.

4. **Exit**  
   - Exit the program.

### Example Usage

1. **Display Cities**  
   - Choose option 1 to view all cities and their coordinates.

2. **Shortest Path Calculation**  
   - Choose option 3 and input:
     - Passenger details (e.g., name and type: student, adult, elderly).
     - Distance between cities.
     - Vehicle type (e.g., mini, standard, luxury).
     - Source and destination cities.
   - The program will:
     - Display passenger details and travel cost.
     - Calculate and display the shortest path with cumulative distances.

---

## Technology Stack

- **Programming Language**: C++
- **Algorithms**:
  - **Haversine Formula** (Distance Calculation)
  - **Dijkstra’s Algorithm** (Shortest Path)
- **Data Structures**:
  - **Linked List** (City Storage)
  - **Graph** (City Connections)
  - **Min-Heap** (Priority Queue for Dijkstra’s Algorithm)

---

## Future Enhancements

1. **Dynamic Data Loading**:
   - Allow users to input city and connection data dynamically via a file or GUI.

2. **Real-Time Distance Updates**:
   - Integrate real-time APIs for accurate distances and conditions.

3. **Additional Features**:
   - Support for additional passenger categories and vehicle types.
   - Multi-language support for user interface.

4. **Visualization**:
   - Provide a graphical representation of the graph and shortest paths.

---

Thank you for choosing **Fast Explorer**! We hope it enhances your understanding of geographical data, travel routes, and cost estimation in a fun and interactive way. **Happy exploring!**