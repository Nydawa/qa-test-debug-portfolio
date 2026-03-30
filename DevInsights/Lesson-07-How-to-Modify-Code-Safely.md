# Lesson 07 — How to Modify Code Safely

Brief lesson summary in 1 or 2 sentences.

Modifying code safely means changing behavior **without breaking existing systems**.  
Instead of removing logic, you **control and wrap it** to keep the game stable.

---

## Concept

- No bugs
- No side effects
- No disruption to other systems

---

## Core Parts

- Part 1: short explanation  
- Part 2: short explanation  
- Part 3: short explanation  

---

## Example

    ```csharp
    public static bool BlockDamage;

    public void TakeDamage(int amount)
    {
    if (!BlockDamage)
    {
        health -= amount;
    }
    }

---

## What Happens Here

A control variable (BlockDamage) is created
The method TakeDamage is called
The condition checks if damage is allowed
If allowed → damage is applied
If blocked → nothing happens

---

## Why It Is Useful

This is important in real modding because:

Helps control behavior without breaking systems
Prevents crashes and side effects
Allows safe interaction with game logic
Used in patches and runtime modifications

---

## Key Idea

- I understood that code is connected and sensitive
- I learned how to block behavior using conditions and flags
- I now see the difference between removing logic and controlling it

---

## What I Still Need to Practice

- I still need to practice identifying safe modification points
- I want to better understand timing and coroutines
- I should test this with different game systems

---

## Link to Real Project Use

Connect this lesson to your real mods.

- PhoneOnSkate → blocking dismount safely using BlockDismount and timing windows
- ProfitCalculator → reading UI data without breaking the game flow
