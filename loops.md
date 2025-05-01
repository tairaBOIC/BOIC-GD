# Loops and Looping

Loops simply repeat themselves for a certain amount of time or conditions.

<br><br><br><br><br>

The easiest Loop is a `while` loop.
```csharp
public class HealthManager{
    
    int health = 10;
    
    public void DamageLoop(){
        
        while (health > 0){
            health -= 1;
        }
        Console.WriteLine(health);
    }
}



```
This will take 1 health away until it reaches 0
then continue

<br><br><br><br><br>

The next loop is a `for` loop

```csharp
public class HealthManager{
    
    int health = 10;
    
    public void DamageLoop(){
        
        for (int i = 10; i > 0; i--){
            health -= 1;
        }
        
        Console.WriteLine(health);
    }
    
}
```

It is slightly more complex so lets break it down

```csharp
for(x; y; z)
```

```chsarp
//  X = the variable we use for counting | usually set to i
//  Y = the condition that we loop again
//  Z = what to do with variable every loop
```
<br><br><br><br>

The final loop you'll need for now is `foreach`

```csharp

int[] damageList;
health = 10;

foreach(int damage in damageList){
    health -= damage;
}


```




### Cheats

`health++;` is the exact same as `health += 1;`
`health--;` is the exact same as `health -= 1;`

`Console.WriteLine("Hello");` will print *Hello* to console 
You can put any variable you want to see information about.
`Console.WriteLine(health);` 
This shows us the health variable.

<br><br><br><br><br><br>



