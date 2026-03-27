# Lesson 04 — Harmony Patches and Hooks

This lesson explains how to hook into game methods using Harmony and modify their behavior.

---

## Concept

Harmony allows a mod to intercept and modify existing game methods without changing the original code.

A patch is attached to a method and runs before, after, or instead of it.

This is how mods “connect” to the game and influence its behavior.

---

## Core Parts

- HarmonyPatch: targets a specific game method  
- Prefix: runs before the original method  
- Postfix: runs after the original method  
- Return control: can block or allow the original method  

---

## Example

    [HarmonyPatch(typeof(GameClass), "SomeMethod")]
    public class Patch_SomeMethod
    {
        static bool Prefix()
        {
            // Block original method
            return false;
        }
    }

---

## What Happens Here

1. Harmony targets a specific method in the game  
2. The Prefix runs before the original method  
3. The Prefix returns false  
4. The original game method is skipped  
5. The mod takes control of the behavior  

---

## Why It Is Useful

- Allows modifying game behavior without editing game files  
- Can block, change, or extend existing systems  
- Essential for interacting with game logic  
- Core mechanic behind most mods  

---

## Key Idea

> Harmony patches hook into game methods and allow modifying or blocking their behavior.

---

## What I Learned

- I understood how patches connect to game methods  
- I learned the difference between Prefix and Postfix  
- I now see how a mod can control game behavior  

---

## What I Still Need to Practice

- I need to practice finding the right methods to patch  
- I want to better understand when to use Prefix vs Postfix  
- I should test patches on different game functions  

---

## Link to Real Project Use

- PhoneOnSkate → uses Harmony patches to block dismount and control phone behavior  
- ProfitCalculator → can use patches to read game data and update UI  
