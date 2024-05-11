# 19AI308-Object-Oriented-Programming-using-CSharp--Exp-8-Name-Hiding-with-interface-inheritance
# AIM:
To implement name hiding with interface inheritance. Aim is to create an interface IMario with a method Ability(). 
Implement this interface in a class Mario and override the Ability() method also to create another class SuperMario that inherits from Mario 
and hides the Ability() method using the new keyword.

## ALGORITHM:
# Step 1:
Create interface IMario with method Ability for Mario classes.

# Step 2:
Mario class implements IMario, defines virtual Ability method.

# Step 3:
SuperMario extends Mario, overrides Ability method with new.

# Step 4:
Instantiate SuperMario and Mario, call Ability on each.

# Step 5:
SuperMario's Ability prints "This is inside SuperMario", Mario's prints "This is inside Mario".

# PROGRAM:
```
Developed by: HARI PRASATH S
Register number: 212222240034
```

```
using System;
{
    
public interface IMario
{
    void Ability();
}

class Mario : IMario
{
    public virtual void Ability()
    {
        Console.WriteLine("Mario's normal ability is Jumping");
    }
}

class SuperMario : Mario
{
    public new void Ability()
    {
        Console.WriteLine("Super Mario's ability is  Flying and shooting fireballs");
    }
}

class Program
{
    static void Main(string[] args)
    {
        Mario mario = new Mario();
        SuperMario superMario = new SuperMario();

        mario.Ability(); 
        superMario.Ability();
    }
}
}
```
# OUTPUT:
![326490903-1dfe74a6-f66b-4017-9d90-c1c30469de69](https://github.com/hariprasath5106/-Exp-8-Name-Hiding-with-interface-inheritance/assets/111515488/f7425046-1592-4ebd-ab32-9f7564e54550)

# RESULT:
Thus, the program has been executed successfully.
