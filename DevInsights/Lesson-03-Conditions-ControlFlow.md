# Lesson 03 — Conditions and Control Flow

This lesson explains how conditions control the flow of a program and determine what code runs.

---

## Concept

Conditions allow a program to make decisions based on values.

They are used to control when something happens, such as blocking an action or allowing it depending on a state.

Control flow defines the order in which code executes.

---

## Core Parts

- if: runs code if a condition is true  
- else: runs if the condition is false  
- ! (not): inverts a condition  
- && (and): requires multiple conditions to be true  

---

## Example

    bool isPhoneOpen = true;
    bool blockDismount = true;

    if (blockDismount && isPhoneOpen)
    {
        return false;
    }

---

## What Happens Here

1. Two boolean variables are defined  
2. The condition checks if both values are true  
3. If true, the code inside the block executes  
4. The function returns false, blocking the action  

---

## Why It Is Useful

- Controls when actions are allowed or blocked  
- Essential for mod behavior (ex: prevent dismount)  
- Allows combining multiple conditions for precise logic  
- Used in almost every system of a mod  

---

## Key Idea

> Conditions decide what code runs based on true or false values.

---

## What I Learned

- I understood how conditions control execution  
- I learned how to combine multiple conditions  
- I now see how logic can block or allow actions  

---

## What I Still Need to Practice

- I need to practice using ! to invert conditions  
- I want to better understand complex condition combinations  
- I should test different logic cases in real scenarios  

---

## Link to Real Project Use

- PhoneOnSkate → uses conditions to block dismount when phone is open  
- ProfitCalculator → uses conditions to filter and calculate values  
