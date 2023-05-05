# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | const var let |

02. What is the definition of a function?

    > |A function performs are particular task. functions always return values. |

03. What are the `SOLID` principles?

    > | Single Responsibility
        Open-closed 
        Liskov Substitution
         Interface Segregation
         Dependency Inversion|

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | fruit.splice(2,1)|

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > | them.friends.push(you)
    you.friends.push(them) ????????????????? |

06. Give an example of a JavaScript `Conditional`:

    > | if (strg ==1){
        return true}|

07. What is the main difference between `parameters` and `arguments`?

    > | A parammeter is used when defining a function. Arguments ARE the values the function receives from each parammeter when function is invoked. |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | Using the code editor feature in the dev tools. You can view your call stack, the breakpoints youve added and even add additional breakpoints|

09. What is the difference between a `primitive` value and a `reference` value?

    > | Primitive: number,string,boolean,undefined,null
    reference: object  |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for (let i = -100; i <= 100; i++) {
  console.log(i); |
