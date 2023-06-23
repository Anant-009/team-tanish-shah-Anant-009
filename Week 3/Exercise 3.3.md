Exercise 3.3:

Code-

function createIncrement()
{
let count=0;
function increment()
{
count++;

    }
        let message=`Count is${count}`;
        function log()
        {
            console.log(message);

        }
        return[increment,log];

}
const[increment,log] = createIncrement();
increment();
increment();
increment();
log();// What is logged?

Explanation:

The output of the above written code is “Output: Count is0 ” , these is a function createIncrement() in which a variable count is declared which stores the value 0. function createIncrement() encloses another function increment() which has an post increment operator for count “count++;” post increment first executes the current stored value and then increases it. Then variable message is stored with `Count is${count}`; in which ${} is a placeholder that is used in template literals.
Again, a function log is declared for printing the the variable message. The in next line increment and log functions are returned. In the next line increment and log have been stored and the function increment(); and log(); are called.
