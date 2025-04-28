# User Input
Simple functions for when a user interacts with the game


<br><br><br><br>

This is how to take an input from a keyboard
```csharp

int health = 10;

void Update(){
  if (Input.GetKeyDown(KeyCode.W)){
      Heal();
  }
}

void Heal(){
  health += 1;
}
```
<br>
Notice that `Update` is being called every frame.
So the computer is constantly checking.

<br><br><br><br>

In this next example, lets Heal when the Key is held down.
```csharp
void Update(){
  if (Input.GetKey(KeyCode.W)){
    Heal();
  }
}
```
<br>
or... When the Key is Released
<br>

```csharp
void Update(){
  if (Input.GetKeyUp(KeyCode.W)){
    Heal();
  }
}
```
