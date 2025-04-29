
# BOIC Simple Game Dev
These are some simple game dev concepts.


## Variables Practive
```csharp
public class Player
{
    bool isAlive = true;
    int health = 10;
    float speed = 2.5f;
    string playerName = "BestPlayer";

    public int maxHealth;
}
```
<br>
<br>

### How it Looks
when you code your variables it will look like this

`bool`
 is your variable type.
 
`isAlive` 
is your variable name.

`=` is equals - basic math

`true` is what the variable is equal to

`;` is how we end every line.

All together we get a variable declaration

```csharp
bool isAlive = true;
```




<br>
<br>
<br>
<br>
<br>



## Variable Types

`bool` is only True or False
```csharp
bool isAlive = True;
```
<br>

`int` is for storing whole numbers
```csharp
int health = 10;
```
<br>

`float` is for storing decimal numbers
```csharp
float speed = 2.5f;
```
<br>

`string` is for storing words or letters
```csharp
string playerName = "LemonMan2543";
```
<br>

Putting `public` in front of any variable, will make it visible to other classes
```csharp
public int maxHealth = 10;
```

<br><br><br><br><br><br>



## Functions
Functions are reusable blocks of code that perform specific tasks.
```csharp
void Heal() {
    health += 2;
}
```
In this example, the players health will increase by 2.
<br><br>

When we want to heal the character, all we have to do is call Heal.
``` csharp
Heal();
```
From anywhere in the script
<br><br>



<br><br><br><br>

We can pass on a variable if we want healing amounts to be different
``` csharp
void Heal(int amount){
    health += amount;
}
```

When we call Heal Player, we need to now give an amount.
``` csharp
    Heal(5);
```
<br><br>
*it's good to note that functions should be named with an uppercase letter `Heal` instead of `heal`*
<br>
*for variables, we start with lowercase `int health`*
*if a variable has 2 words like Max Health we write like this `maxHealth`* No space


<br><br><br><br><br><br>


You're probably wondering what `void` means.

`void` says what variable type to return to the caller.

`void` means, return nothing to the caller.

<br><br>
But we can send data back

This sends back the new health after adding 2
``` csharp
int Heal(){
    health += 2;
    return health;
}
```

<br><br><br><br>

# ALL DONE GUYS
When we put everyhting together we get...

```csharp
public class Player : MonoBehaviour
{
    bool isAlive = true;
    int health = 10;
    float speed = 2.5f;
    string playerName = "BestPlayer";
    public int maxHealth;

    
    void Heal(int amount){
        health += amount;
    }
}
```
<br><br><br><br><br><br>
