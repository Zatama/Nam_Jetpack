# Bucket update Notes
* **Jumppacks**
    - **Functionality**
        + Keybinding
            +   4 key bindings (although you only need 2 to function). They are **jump**,**cycle left**.**cycle right** (you only need one of those two,or both),**show energy**. You can set them in ***controls>configure addons***
        +   How it works
            +   First I will explain what each jumppack has. Each jumppack has the following properties
                1. **Display name***: lol,what you see in arsenal
                2. **Is it a jumppack**: Tells the scripts is this backpack a jumppack.
                3. **Spam delay**: basicly how many seconds till you can jump again assuming all other prerequists are meet. This prevents well...spamming.
                4. **Energy Capacity**: Each jumppack has a energy capcity, think of it as fuel. Each jump costs a certain amount, some more then others or less then others.
                5. **Energy Recharge**: A fixed value at energy/second for energy regeneration. Some jumppacks have higher or lower recharge rates.
                6. **Jump Types**: A huge list of availible jumps a jumppack has. Some have 1,2,3, or even 4+ jumps. Each jump has a value to indicate its **its name**,**forward velocity**(X-velocity in direction of jump),**verticle velocity**,**angle**(I.E 90 left, or 90 rights, or 180 which is reverse, or even 45 degrees left), **is it a directional jump?**(if so it will ignore the angle and jump you the direction you are looking but you must have a weapon out so if you are surrendering or captured you cant. You can have you weapon pointing one way and you looking another and you will jump the direction you are looking.), and finally **can prone jump**(some jumps prevent young grasshopper mode).
                7. **Ignite sound**: sound to play when you jump.
                8. **Idle sound**: sound that is played while you are jumping.
                9. **Landing sound**: sound to indicate when you have landed.
                10. **effect**: What particle effect function to play while you jumping and when you land.
                11. **effect position**: Where on the body this effect will be.
            +   If you select jump left it basicly goes up the list, and if you cycle right it will go down the list, both will loop around so you only really need one bound.
            +   The system will detect when you go into arsenal(ACE or BI) or if you loadout changes. NOTE: if you drop the jumppack and pick it up it will **NOT** give you your energy back (RIP cheaters). You have to either change backpack complety or go to arsenal to reset the energy.
            +   When you press to jump the system will check various conditions such has do you have enough energy, are you in a vehicle, are you spam jumping, do you have a weapon out, are you prone and so on. Once you pass all conditions you will be allowed to jump. 
            +   When you are jumping **you are invincible**. I will try and make it so in the future you can take damage, but for now this will have to do. 
            +   When you use directional jump, if you get clipped on something and jump for less then .1 seconds(basicly you didn't jump) it will not comsume energy(Spam delay still applies though).
    - **Jumppacks**
        + ***Republic***
        +   All the republic ones have the same sound and effects for now.  
            + CDV-21 [Low Capacity]
                + **Energy Capcity**:60
                + **Energy Recharge**:10 energy per second
                + **Spam delay**: 0.05 seconds
                + **Jumps**
                    +   Forward jump, forward velocity =10.1,verticle 21.5, costs 50, goes forward, cant prone jump
                    +   Short jump, forward velocity =12,verticle 10, costs 30, goes forward, cant prone jump
                    +   left jump, forward velocity =10.1,verticle 21.5, costs 50, goes left, cant prone jump
                    +   right jump, same as left jump but right lol
            + CDV-21 [High Capacity]
                + **Energy Capcity**:150
                + **Energy Recharge**:4 energy per second
                + **Spam delay**: 0.3 seconds
                + **Jumps**
                    +   Short jump, forward velocity =12,verticle 10, costs 30, goes forward, cant prone jump
                    +   reverse jump,same as short but backwards
                    +   up jump, forward velocity =3,verticle 20, costs 30, goes up, cant prone jump
                    +   down jump,same as up but goes down
            + CDV-21 [Normal Capacity]
                + **Energy Capcity**:100
                + **Energy Recharge**:4 energy per second
                + **Spam delay**: 0.2 seconds
                + **Jumps**
                    +   Forward jump, forward velocity =10.1,verticle 21.5, costs 50, goes forward, cant prone jump
                    +   Short jump, forward velocity =12,verticle 10, costs 30, goes forward, cant prone jump
            + CDV-21LR [Normal Capacity]
                +   Has same LR as CDV-19m
                + **Energy Recharge**:3.6 energy per second(10% less then CDV-21)
                + 5% more room in inventory
                + Rest is the same as CDV-21
            + CDV-21 [Titan Mode]
                + **Energy Capcity**:100
                + **Energy Recharge**:5 energy per second
                + **Spam delay**: 0.2 seconds
                + **Jumps**
                    +   Forward jump, forward velocity =10.1,verticle 21.5, costs 50, goes forward, prone jump
                    +   Short jump, forward velocity =12,verticle 10, costs 30, goes forward, cant prone jump
                    +   Directional jump,forward velocity=18,verticle=5, cost 30 ,goes in direction you are looking,prone jump
                + has grey texture
            + CDV-21PP [Pilot Mode]
                + **Energy Recharge**:6 energy per second   
                 + **Jumps**
                    +   Directional jump,forward velocity=18,verticle=5, cost 30 ,goes in direction you are looking,prone jump
                + has grey texture
                + has same LR as cdv-19m
            +   CDV-21 [One Time]
                + **Energy Capcity**:3
                    + **Energy Recharge**:0 energy per second
                    + **Spam delay**: 2 seconds
                 + **Jumps**
                    +   Forward jump, forward velocity =10,verticle 5, costs 1, goes forward, prone jump 
                + Basicly a parachutre verision of the jumppack.
                