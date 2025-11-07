# 📊 Sorting Algorithm Comparison Visualizer

A modern, interactive, and responsive web application that visualizes 10 popular sorting algorithms running side-by-side. Built with raw JavaScript, HTML5 Canvas, and Tailwind CSS, this tool provides deep insights into how different algorithms operate under various conditions.

![A dashboard showing multiple sorting algorithms like bubble sort, merge sort, and quick sort, running side-by-side on colorful bar graph visualizations.](https://placehold.co/800x400/1f2937/f3f4f6?text=Sorting+Visualizer+Dashboard)

## ✨ Key Features

* **Simultaneous Visualization:** Run up to 10 algorithms concurrently on identical input arrays.
* **Real-time Controls:** Pause, Resume, and Cancel active visualizations instantly.
* **Robust Metrics:** Tracks execution time, number of comparisons, swaps/writes, and frames rendered for every algorithm.
* **Diverse Input Distributions:** Test algorithms against different data shapes:
    * Random
    * Reversed
    * Nearly Sorted (10% noise)
    * Few Unique Values (k=5)
    * Gaussian Distribution
* **Detailed Visuals:**
    * Color-coded states: Primary (Blue), Compare (Yellow), Swap (Red), Sorted (Green), Pivot (Orange).
    * Special overlays for non-comparison sorts (Counting, Radix, Bucket) showing internal state without distorting the main array.
    * Partition highlighting for Quick Sort.
* **Shareable States:** Settings (speed, size, selected algorithms) are persisted to `localStorage`.

## 🚀 Getting Started

This project is entirely client-side and requires no build tools, package managers, or local servers.

### Prerequisites

* A modern web browser (Chrome, Firefox, Edge, Safari).
* An active internet connection (required for loading Tailwind CSS and Google Fonts via CDN).

### Installation & Running

1.  Download the `sorting-visualizer.html` file.
2.  Open the file directly in your web browser.

That's it!

## 🧮 Supported Algorithms

The visualizer includes standard implementations of the following:

| Algorithm | Type | Best for... |
| :--- | :--- | :--- |
| **Bubble Sort** | Comparison | Educational purposes; nearly sorted data. |
| **Selection Sort** | Comparison | Small memory footprint; minimizing writes. |
| **Insertion Sort** | Comparison | Small or nearly sorted datasets. |
| **Merge Sort** | Comparison | Predictable O(n log n) performance; stable sorting. |
| **Quick Sort** | Comparison | General purpose, high-speed sorting. |
| **Heap Sort** | Comparison | Systems requiring O(1) auxiliary space. |
| **Counting Sort** | Integer | Small integer ranges. |
| **Radix Sort (LSD)** | Integer | Large lists of integers; avoids direct comparisons. |
| **Bucket Sort** | Distribution | Uniformly distributed data. |
| **Shell Sort** | Comparison | Medium-sized arrays; improvement over Insertion Sort. |

## 🛠️ Technologies Used

* **HTML5 Canvas:** High-performance 2D rendering of bars.
* **Vanilla JavaScript (ES6+):** `async`/`await` for animation loops and concurrency management.
* **Tailwind CSS (CDN):** rapid, responsive UI styling.

## 🎮 Controls Guide

* **Array Size:** Adjusts the number of elements (10 to 300).
* **Delay (ms):** Controls animation speed. Set to 0ms for maximum speed (limited only by browser frame rate).
* **Seed:** Enter a number to generate reproducible random arrays. Leave empty for a random seed every run.
* **Run Selected:** Launches only the checked algorithms.
* **Run All:** Launches all 10 algorithms simultaneously.

## Demo
https://swapnilgopale.github.io/Sorting-Algorithm-Visualizer-v2/

## 📄 License

Distributed under the MIT License.
