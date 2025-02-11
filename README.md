# PHP foreach loop modification during iteration
This repository demonstrates a common error in PHP where modifying an array during a foreach loop leads to unexpected results.  The `bug.php` file shows the incorrect approach, while `bugSolution.php` provides the corrected version.

The issue arises because `unset()` directly manipulates the array's internal pointer, potentially skipping elements.

The solution avoids this by creating a copy of the array or iterating in reverse.