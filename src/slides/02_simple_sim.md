# Simple Simulation of PI

## The Method

Estimating PI with the Monte Carlo algorithm

<table>
<tr>
<td>
  <img src="img/basic_example_monte.gif" />
</td>
<td>
  <img src="img/pi_simulation.png" />
</td>
</tr>
</table>

---

## The Scripts

### The Core Calculation

 - basic R script
 - two arguments:
   - a starting condition
   - number of iterations (throws)
 - counts number of throws inside circle
 - uploads result into S3

---

## The Scripts

### The Executor

  - Python script (boto library is gold standard)
  - Submits a set of jobs
  - Monitors output bucket
    - periodically updates estimate of &pi;
  - Exits when there are no more running jobs
  - Prints final result

---

## Execution

???
On-screen demo

---

