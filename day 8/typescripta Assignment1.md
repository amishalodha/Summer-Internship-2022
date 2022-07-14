 # Typescript quiz (Basic Level -1) 

 Q 1  What are the basic data types in TypeScript?
 * In typeScript, type System represents different types of datatypes which are supported by TypeScript. The data type classification is as given below:



    * Number - It is used to represent both      Integer as well as Floating-Point numbers
   	 * Boolean	Represents true and false.

    * String-It is used to represent a sequence of characters.
    * void	Generally used on function   return-types.
    * Null-It is used when an object does not have any value.
     * Undefined-Denotes value given to uninitialized variable.
    * Any-If variable is declared with any data-type then any type of value can be assigned to that variable.

Q 2 What is Generic data type.?
   * It creates a component that can work with a variety of data types rather than a single data type. It allows users to consume these components and use their own types.

   ```javascript
   function identity<T>(arg: T): T {    
    return arg;    
}  
```
Q 3 What is type inferring in TS.
* In TypeScript, there are several places where type inference is used to provide type information when there is no explicit type annotation. For example, in this code
```javascript
    var a = "some text";
var b = 123;
  a = b; // Compiler Error: Type 'number' is not assignable to type 'string'
```

Q 4 What are the possible ways to define typing for functions?
* Three Possible ways:
   * Method Signatures
The method signature syntax is probably the most straightforward to use. When defining an object type, its methods can easily be described by providing signatures as follows:

 ```javascript 
 interface Date {
  toString(): string;
  setTime(time: number): number;
  // ...
}
 ```

* Function Type Literals
 They're typically used in the signature of a higher-order function, that is, a function which accepts functions as parameters or which returns a function:
 ```javascript
interface Array<T> {
  sort(compareFn?: (a: T, b: T) => number): this;
  // ...
}
```

* Object Type Literals with Call or Construct Signatures
  In JavaScript, functions are nothing but special objects than can be called. This fact is reflected in the syntax of object type literals: they describe the shape of an object, which also happens to have a call signature:

 ``` javascript interface RegExpConstructor {
  // Call signatures
  (pattern: RegExp): RegExp;
  (pattern: string, flags?: string): RegExp;

  // ...
}
```
Q 5 How to define Generic type for Classes.
  * TypeScript supports generic classes. The generic type parameter is specified in angle brackets after the name of the class. A generic class can have generic fields (member variables) or methods.

  
Q 6 Define the types in typescript for the given following JavaScript code.
```javascript
  
  class List{
    name: string;
    description: string;
    done: boolean;
  }
 var todos :List[]= [];
 function add(name:string , description :string) :number {
    return todos.push({
        name: string ,description:string,
        done: false,
        });
    }
function remove(index:number) : List[]{
        return todos.splice(index, 1);
    }

    function list():void {
    todos.forEach(function(todo:List,index:number) 
    {
        console.log(index + " -" + todo.name);
        });
        }
        function update(index:number , name: string, description:string):List {
            todos[index].name = name;
            todos[index].description = description;return todos[index];
            }
            console.log(add("work complete"));
            list();

```

