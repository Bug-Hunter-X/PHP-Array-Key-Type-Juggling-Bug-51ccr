# PHP Array Key Type Juggling Bug

This repository demonstrates a subtle bug in PHP related to array key comparisons and type juggling.  The `bug.php` file contains code that incorrectly uses loose comparison (`==`) when checking for the existence of an array key. This can lead to unexpected results when keys are strings that can be type-juggled to integers.

The `bugSolution.php` file provides a corrected version that uses strict comparison (`===`) to prevent this issue.  This ensures that keys are checked against values of the exact same type, preventing type-juggling related errors.