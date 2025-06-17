# ConvexityCheckerParallel
This Java project checks whether a given polygon is **convex** or **concave** using **parallel programming** (multithreading). The algorithm uses the **cross product method** to determine the direction of turns and distributes the workload across multiple threads for performance.
 Key Features

- Detects convex or concave shape given a list of 2D points.
- Uses cross product logic to determine angle orientation.
- Implements multithreading with `ExecutorService` for efficiency.
- Handles cyclic point indexing (wrapping) in polygon structure.

 How It Works

- Each thread processes a subset of the polygon's vertices.
- The cross product of each triplet of points is calculated.
- The signs of the cross products are compared to determine consistency.
- If a sign mismatch is detected across threads, the polygon is concave.

 Example Output
Quadrilateral: Convex
Pentagon: Concave

 Technologies
Java 8+
java.util.concurrent
Object-oriented and thread-safe design

 Sample Polygons
Convex quadrilateral: square or rectangle

Concave pentagon: arrowhead-shaped

 How to Run
Clone the repository:

git clone https://github.com/yourusername/ConvexityCheckerParallel.git
