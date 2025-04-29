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
<br>
x: The variable we use for counting, usually set to
<br>
y = check this every loop to see if loop should continue.



