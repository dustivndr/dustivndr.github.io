---
title: cowboy-cpp
layout: projects
project-id: 1
---

# Cowboy C++, Battle and Quiz Game

<u>Project status: Ongoing</u>

Simple ASCII battle and quiz game in C++, works in Windows/Linux Terminal (at least in Fedora, where I write the code).

This is a small project created for fun and is not part of any university coursework.

# Gameplay

This information is also available on the wiki page [here](https://github.com/dustivndr/cowboy-cpp/wiki).

You're a Cowboy, wandering through vast land, encountering different bosses, ranging from the easy ones to the hardest ones.

The gameplay is simple; you move only forward, and at a random time, you will encounter a boss, starting from the easiest one.
The more bosses you discover, the harder the difficulty will be. You and the boss only have 2 choices: attack or defend.

## Attack

When you attack the boss, there's a chance for the attack to be critical (deals double damage) or 0 (attack fails).
Attacking an easy boss is 100% guaranteed to succeed (no fail attack).

### Boosted Attack

This is where the quiz part is.<br />
You can double the attack damage by answering one quiz question correctly.
The Attack Booster can only be used once per battle. How long the effect will last depends on the boss's difficulty.

<table>
    <thead>
        <tr>
            <th>Difficulty</th>
            <th>Apply to</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Easy</td>
            <td>1 move</td>
        </tr>
        <tr>
            <td>Medium</td>
            <td>2 move</td>
        </tr>
        <tr>
            <td>Hard</td>
            <td>4 move</td>
        </tr>
    </tbody>
</table>

A "move" refers to each time you choose to attack or defend.

- Every attack or defence action counts as one move.
- For example, if you encounter a medium boss and use the attack booster:
  - First move: attack (damage is doubled)
  - Second move: defend
  - Third move: attack (damage returns to normal)

## Defend

When defending, the player has a 50% chance to block all damage or reflect the boss's attack at them.
For hard bosses, only 50% of their attack damage is reflected when defending.

## Player's Health

While wandering (not in battle), the player's HP automatically increases by 1 point every second, up to a maximum HP limit.
