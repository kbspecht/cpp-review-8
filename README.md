# cpp-review-8

CPU starts execution at top of main/terminates at end, set of statements executed is execution path, straight line program takes direct path, control flow statements let programmer change path of execution through program
Flow control statements include conditionals that execute if condition is met (if, else, switch), jumps that tell CPU to start executing at some other location (goto, break, continue), function calls that jump to some other location & back (function calls, return), loops thatexecute some line of code repeatedly until some condition is met (while, do while, for, ranged for), halts that terminate program (std::exit(), std::abort()), exceptions that handle errors (try, throw, catch)
Conditions made with if/else if/else, can have nested statements (make sure else/else if is matched up with appropriate if)
Null statement exists of only ; (used when language needs statement but programmer doesn't need one), avoid putting ; at end of if statement or null statement results
Use == instead of = in if (using x=0 sets x to 0 then evaluates x)
If evaluated at runtime, if conditional is constexpr then if evaluated at compile time
Switch statement uses different cases depending on switch variable, executes code (code in case statement not nested scope for switch) for case label of value (ex. case 1) corresponding with switch variable value (else default case), all case labels must be unique, if no cases met/no default case then none of switch block is executed, can use return at end of case or break to exit block/continue (needed to stop execution of following cases, can add [[fallthrough]] comment to indicate that subsequent case is meant to be executed), place multiple case labels in sequence for statement executed under multiple cases, can declare but not initialize variables inside switch (can create additional block in case statement if initialization needed)
Unconditional jump causes execution to jump to another spot in code (for all cases), implement via goto statement/jump to spot identified with statement label (statement made without indent, has function scope so visible throughout function), goto statement/statement label must be in same function, should generally avoid (makes code execution messy, use when you need to exit nested loop but not function)
Loop lets piece of code execute repeatedly until condition met, condition based on loop variable (should be signed as unsigned can overflow, can use % to specify certain iterations), infinite loop executes forever, nested loop inside other loop, while statement executes as long as condition true/not at all if condition false, do while statement executes once then continues to execute as long as condition true/stops if condition false, for statement has 3 part condition (initial state of loop variable, condition for exiting loop checked in each iteration, end expression that increments/decrements loop variable, can omit conditions/add them manually in block, can also have multiple loop variables), make sure loop variable is accurate (not off by one), don't give loop variable scope outside loop unless necessary, break causes loop to end early/return terminates entire function loop is in, continue proceeds to start of next loop iteration/ends current one (use carefully)