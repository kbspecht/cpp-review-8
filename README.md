# cpp-review-8

CPU starts execution at top of main/terminates at end, set of statements executed is execution path, straight line program takes direct path, control flow statements let programmer change path of execution through program
Flow control statements include conditionals that execute if condition is met (if, else, switch), jumps that tell CPU to start executing at some other location (goto, break, continue), function calls that jump to some other location & back (function calls, return), loops thatexecute some line of code repeatedly until some condition is met (while, do while, for, ranged for), halts that terminate program (std::exit(), std::abort()), exceptions that handle errors (try, throw, catch)
Conditions made with if/else if/else, can have nested statements (make sure else/else if is matched up with appropriate if)
Null statement exists of only ; (used when language needs statement but programmer doesn't need one), avoid putting ; at end of if statement or null statement results
Use == instead of = in if (using x=0 sets x to 0 then evaluates x)
If evaluated at runtime, if conditional is constexpr then if evaluated at compile time