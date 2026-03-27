# Lesson 04 — Methods & Game Calls

A game runs through methods (actions).

## Core idea
A method is an action:
- TakeDamage()
- OpenPhone()
- Dismount()

The game constantly calls methods.

## What a mod does
A mod connects to these methods and can:
- Listen
- Modify
- Block
- React

## Game Call
When the game executes:
player.TakeDamage();

This is a Game Call.

## Harmony system

### Prefix
Runs BEFORE the method.

Can block the action:
return false;

### Postfix
Runs AFTER the method.

Used for logging or reacting.

## Example
if (Core.BlockDismount)
{
    return false;
}

This blocks the dismount.

## Mental model
Game → Method → Action

Modded:
Game → Method → Mod → Action or Block

## Key idea
A mod sits between the game and its actions.
