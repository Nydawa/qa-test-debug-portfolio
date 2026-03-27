# Lesson 03 — Conditions and Control Flow

Conditions allow a mod to make decisions.

## Core concepts

* `if`: executes code only if a condition is true
* `bool`: true / false values used in logic
* `return`: stops execution and returns a result

## Example

```csharp
if (Core.BlockDismount)
{
    return false;
}
```

## Behavior

* `return true` → allow game behavior
* `return false` → block game behavior

## Negation

```csharp
if (!Core.BlockDismount)
{
    return true;
}
```

* `!` means NOT (inverts a boolean value)

## Combined conditions

```csharp
if (Core.BlockDismount && Core.PhoneOpen)
{
    return false;
}
```

* `&&` means AND (both conditions must be true)

## Simplified logic

```csharp
return !Core.BlockDismount;
```

## Key idea

A mod is a decision system.

It checks conditions and chooses to allow or block game actions.
