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
for (int i = 0; i > 0; i++){
  health -= 1;
}
```

It is slightly more complex so lets break it down

```csharp
for (int )
