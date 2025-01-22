# NPC Dialogue and Quest System

## Overview
This project involves creating an NPC dialogue system for a game. The dialogue is structured using XML files, and NPCs offer quests with specific objectives, character interactions, and rewards. The current work is based on templates from existing NPCs, and new quests will be added progressively.

The XML files define the dialogues, quest structures, and rewards, allowing the game to dynamically handle quests and NPC interactions.

## Quest List

### Quest #1: Secluded Sands
**Fishing Level Requirement**: 200  
**Quest Title**: Secluded Sands  
**Quest Given By**: Padean Maclir  
**Objective**: Interact with Mac an Iasgair

#### Quest Dialogue:
- **Padean Maclir**:  
  _First time we have talked... Can you do me this favor?_  
  (Continue) (SKIP)  
  _A fellow fisher went to discover Skye... I need that assurance._  
  (Continue)

- **Mac an Iasgair**:  
  _You are not from around here... Who sent you?_  
  (Continue)  

#### Quest Completion:
- **Padean Maclir**:  
  _Is he alive? He is! I cannot thank you enough, ___(character name)___..._  
  **Rewards**:  
  - EXP: 250,000

---

### Repeatable Quests

#### Daily: Bronze Offering
**Fishing Level Requirement**: 200  
**Quest Title**: Daily: Bronze Offering  
**Objective**: Turn in ten bronze marks of Nodens and five auroral trout

#### Quest Completion:
- **Mac an Iasgair**:  
  _As promised, here is your reward._  
  **Rewards**:  
  - Tide Bounty Bag

## XML Structure
The quests and NPC dialogues are structured in XML format. Below is an example of the XML content used for these quests.

```xml
<quest>
  <id>1</id>
  <title>Secluded Sands</title>
  <npc>Mac an Iasgair</npc>
  <dialogue>First time we have talked...</dialogue>
