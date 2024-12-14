# Go Race Condition

This repository demonstrates a simple race condition in Go.  The `bug.go` file contains code that uses multiple goroutines to increment a counter without proper synchronization, leading to an incorrect final count. The `bugSolution.go` file provides a corrected version using a mutex to prevent race conditions.

**How to Run**

1.  Clone this repository.
2.  Navigate to the repository directory.
3.  Run `go run bug.go` to see the race condition in action.  The output will likely be less than 1000.
4.  Run `go run bugSolution.go` to see the corrected version with the correct output (1000).