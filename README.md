# Moveset notes for pokémon gen II

This is a work in progress,
for the latest version see https://github.com/cdn-lnk/pkmn-genII-moveset-guide

## Stats

* __Start considering base stats__, a level 100 shuckle with max individual and effort values has 118 special attack while an abra with zero individual and effort values has the same 118 special attack at level 54.

* __Think in terms of effective stats__, a pokémon with 200 attack using a move with power of 25 has equivalent damage to a pokémon with 100 attack using a move with power of 50. Similarly, 200 hp pokémon with 100 defense is roughly the same as 100 hp pokémon with 200 defense. A good approximation is:

$$\text{effective attack} \approx power \times attack$$

$$\text{effective defense} \approx hp \times defense$$

* __Focus on special OR physical attack, not both__, choose moves that fit whichever is higher.
  * What if your physical attack is higher than you special attack, and following this advice you only learn physical moves, what happens when your opponent uses a pokémon with very high physical defense but very low special defense? You change to a pokémon with high special attack.

* __HP is better than defense__, it may be hard to predict what moves your opponent has, since hp doesn't split in special and physical it is preferable over defense.

## Role

* __Know your role!__ Choose a role that match the pokemon status.

* __Sweeper__: combines high speed with high effective attack. Usually fragile and dependant on type advantage and STAB. Powerfull moves are preferable over moves with many power points.
  * They don't tend to survive the rounds needed to do proper stage buffs (e.g.: belly drum) themselves, but they are great combos with batton pass if someone else can setup the stats for them.

* __Wall__: combines high speed and effective defense. Leads to longer battles, great holders of utility moves and baton pass since have plenty of a time to setup.

* __Tank__: combines, high effective attack and effective defense, tends to longer battles.

* __Choose moves based on roles__: A sweeper with no strong moves or a wall without utilities are bad strategies.

* __Pokémon need to survive long enough to fulfil its role__: If you lose 90% of your hit points in a single turn something is wrong.

## Types

* __Pokémon are weak against moves, not aginst other pokémon__: A gyarados without water moves is a smaller threat to a typhlosion than a pikachu that knows surf.

* __STAB is OP!__ Types are divided in two categories: physical and special. Due to STAB physical types benefit more from physical attacks while special types benefit more from special attacks.
  * This means that a a water pokémon which has physical attack greater than special attack will never reach the move full potential, in other words, it should be considered more for its defensive capabilities.

__physical__|__special__
-|-
bug|dark
fighting|dragon
flying|electric
ghost|fire
ground|grass
normal|ice
poison|psychic
rock|water
steel

* __Some types only have physical (or special) weaknesses__, this gives them an preference for a certain type of defense: dark, electric and normal benefict more from physical defense while dragon, ground and water more from special defense.

* __Avoid redundancy__: Learning ember, fire blast, flamethrower and flame wheel all at the same time isn't the best idea.

* __Maximize coverage__: In a less obvious way earthquake and surf are the same move. They have almost the same power, and are strong against almost the same types of pokémon.

## Moves

* __Power is important, but so are power points, turns and accuracy__

#fixme:
$$potential = \frac{points \times power \times accuracy}{turns}$$

* __Pokémon that lasts longer needs more power points__, a snorlax with blizzard, zap cannon, hyper beam and rest may run out of power points.

* __Status ailments priorities__: Since only one can be inflicted at a time, save it for the better ones.
The priority usually is strong sleep, frozen, weak sleep, paralysis, burn and poison.

Notes:
1. Freeze and sleep increase catch rate of wild pokémon and forbid fleeing.
2. Sleep is way more reliable than freeze, but freeze comes with damage.
3. In battle tower sleep is limited to 3 turns max (number in parenthesis at the table below).
4. Burn is a poison with physical damage reduction.
5. Think of poison as a 8 turn destiny bond with immediate damage. It is a multi turn strategy and inherit the disadvantages of one (consider moves like mean look or spider web).
6. Badly poison is demoted to poison if pokémon switch.
7. Badly poison kills target after 6 rounds if there is no cure.
8. As rule of thumb status infliction with 100% accuracy are overpowered.
9. We did not consider tri attack in calculations

__status__|__average damage reduction__
-|-
freeze (except blizzard)|50%
blizzard|41%
spore|50% (33%)
lovely kiss & sleep powder|46% (30%)
hypnosis|43% (27%)
sing|42% (26%)
paralysis|25%
burn|50%
badly poison|0%
poison|0%

* __Heal is only advantegeous if you have high defense__: If you die in one hit it doesnt matter if you heal.

* __Recoil only with heal__: thus recoil indirectly needs high defense.

* __Flinch increases damage by probablility__: and does not stack with kings rock.

* __Save TMs for later__: If you can get stronger by other means, like leveling up or using items, save your TM for later (exception are buyable TMs).

## The power of money

* __If you can get the effect with items, do it__

Example #1: A cloyster that knows withdraw versus a cloyster that doesn't know withdraw but trainer uses x defense. In both cases cloysters ends with +1 defense stage after one turn, however the latter has one extra slot for learning another move.

Example #2: King's rock provides flinch.
  * Fixme: Is it better to have a powerful move with king's rock or have low kick plus black belt? #todo: math

Example #3: Potions vs rest.

Item|Replaceable moves
-|-
guard spec|mist
miracle berry(rare as f***)|safeguard(kinf of)
quick claw**|quick attack, extreme speed(kind of)
king's rock|flinch

Still slower than extreme speed and quick attack
X special raises both special attack and special defense.
X Accuracy completly ignores checks.

## Multi turn (not to be confused with muti hit)

* __Multi turn is usually bad__: Suppose your dugtrio uses dig. The opponent knows what happens next and has one turn to plan for it. He could change for a gyarados which has immunity against dig and water moves against dugtrio. The more turns you need to accomplish something the more predictable and counterable (by switching for example) you are.
  * #fixme what about lose pp?

* __Burst is best than over time__: Suppose your charizard can knockout the opponent by using flamethrower once or by using thunder punch twice. Choosing thunder punch gives the opponent the chance to switch and save that pokémon for later, or even heal it.

## Stages

The numbers in the table are how many moves you gotta hit for the turns lost during raise to be worth it.
Assuming most efficient way is first raise than attack. Can be very useful for preventing heal, you need a OHKO though.

* __Be aware of the 999 stats cap__: Suppose pokémon A has 300 attack and pokémon B has 200 defense. In this case pokémon A has advantage of 1.5. If pokémon A decides to raise its attack by 6 stage and pokémon B decides to raise its defense 6 stages, now both of them are at 999 and pokémmon A no longer has a stat advantage.
  * The same __doesn't__ apply for lowering stages.

* __Lowering enemy stages require can't escape moves__: Let's imagine our plan is to use screech twice (while taking some damage) and then in the third round deal a killing blow. Sounds great! But what happens if the opponent changes pokémon after the second round? It resets all stats, effectively wasting our two turns.
  * To use a multi turn strategy it is __indispensable__ moves that forbid the opponent of escaping (mean look and spider web).

* __Don't start never ending battles__:
+1 -1 +1 -1 +1 -1

* __Critical hit sucks!__: and so does Focus energy. Get a dire hit and save a move slot. But dire hitis still not good, see below:

stage|probability|average damage increase
-|-|-
0|1/16 (6.25%)|0
+1|1/8 (12.5%)|54/51 (5.88%)
+2|1/4 (25%)|60/51 (17.65%)
+3|1/3 (33%)|64/51 (25.49%)
+4|1/2 (50%)|72/51 (41.18%)

Using x-attack or x-special once increases your average attack by 50%.

Notes:
1. it ignores burn.
2. it ignores reflect and light screen.
3. it ignores stage modifiers if their defense is higher than your attack (good against walls that raise defense).
4. it ignores evasion (test this)
5. it doubles both special and physical attacks while swords dance only raises one of them. This is not valid bacause you know your stats so you should know what you want use.
6. There is no max stat cap for critical hits (not realistic)

* __X-accuracy is anti-game__: There are no moves that raise accuracy but if x-accuracy is used once all accuracy checks, future and past, are ignored.
  * Imagine using flash for 6 turns to get max evasion and then have it all negated in a single turn by x-accuracy. What's worse you lost a move slot.

> This renders flash, kinesis, sand attack and smoke screen, double team, minimize, sweet scent, mind reader and lock on useless.

Notes:
1. Despite smaller values evasion works as both physical and special and __prevents side effects__.
2. There is no x-evasion;

* __Raising and lowering speed__

If you already attack first there is no point in it.
If you die in one hit there is no point in it.
Maybe batton pass to a slow pokémon?
Agility is the only raising one and it is by +2.
string shot -1
cotton spore, scary face -2
No idea on the subject

* __Scenario 1, raising your attack__: Meditate, sharpen and growth suck! Get a x-attack or x-special and save a move slot.
  * Belly Drum is always worth it unless you can get knocked out in one hit.

stage|multiplier|ideal turns (x-attack & x-special)|ideal turns (swords dance)|base stat for 999 cap
-|-|-|-|-
0|1|1-3|1-2|----
+1|3/2|4-5||----
+2|2|5-7|3-4|----
+3|5/2|7-9||----
+4|3|9-11|4-6|400
+5|7/2|11-13||333
+6|4|13+|6+|286

* __Scenario 2, lowering enemy's defense__: Always worse than raising your attack since: 1) you need one extra turn for a can't escape move and 2) you need to re-setup for each pokémon the opponent sends.
  * The only advantage I can see is that there is no min stat cap, so (e.g.) mewtwo is stronger against one opponent with minimun special defense than it is with maximum special attack (due to the 999 cap). Not realistic though.
  * This means you need to hit the same pokémon 13+ times and +5 turns of preparation this means 18 turns against the same pokémon!!!! << What I wrote here?

stage|multiplier|leer, tail whip|screech
-|-|-|-
0|1||
-1|3/2|
-2|2||
-3|5/2||
-4|3||
-5|7/2||
-6|4||
 
* __Scenario 3, raise your defense__: Harden and withdraw suck! Get a x-defense and save a move slot.
> Defense curl doesn't suck, it combos with rollout.

stage|multiplier|x-defense|amnesia, barrier, acid armor|don't go if you have more than
-|-|-|-|-
0|1|||----
+1|3/2|||----
+2|2|||----
+3|5/2|||500
+4|3|||400
+5|7/2|||333
+6|4|||286

#todo: idea for filling the table use a blissey and see maximum hp that can be obtained. and consequently number of turns.
$$\left<damage\right> = \frac{1}{N} * \sum_{n=0}^{N}\left(\frac{2}{2+n}\right)^n$$

* __Scenario 4, lowering enemy's attack__: See Scenario 2, lowering enemy's attack arguments.

stage|multiplier|growl|charm
-|-|-|-
0|1||
-1|3/2|
-2|2||
-3|5/2||
-4|3||
-5|7/2||
-6|4||

* __Spread stages uniformly?__: A raise plus a lower is always better than two raises or two lowers.
  * Is it worth the extra slot though? #DoTheMath!

* __Which is better? raise attack or raise defense?__: I don't know yet. #DoTheMath!

* __Which is better? lower attack or lower defense?__: I don't know yet. #DoTheMath!

* __Baton pass is actually good__

* __Roar counters batton pass__

## Items

* __Leftovers is the cookie cutter strategy__

Leftover is considered the best item, except if you expect your pokémon to die fast. Generally heals more than berry/berry juice/gold berry and the amount healed offsets damage increasing items.

Other good items are: quick claw, bright powder, scope lens(?), focus band and king's rock.

* __Miracle berry for the win__

Why cure only one status ailment if you can cure all of them?

Note: In battles where you can not repeat items and when you are sure of some specific condition it may be better to save mystery berry. For example, if you plan to use rest it is better to have a mint berry or if you bitter berry for thrash.

* __Stat enhancing items are overpowered__

They just are, particularly thick club.

item|pokémon
-|-
stick/leek|farfetch'd
light ball|pikachu
lucky punch|chansey
metal powder|ditto
thick club|cubone and morawak

* __Type enhancing items are overestimated__

A level 100 blissey with maximum effort values and individual values have staggering 713 hit points, making her the pokémon with more hp of all.

This means that the maximum damage due to type enhancing items is 64 hp

$$713 = 649*1.1 = 649 + 649*0.1 = 649 + 64$$

If blissey holds leftovers it would heal 44 hp back resulting in a net damage of miserable 20 hp.
However a type enhancing items can be crucial if it guarantees a 1hko.

## Unique moves

* __Don't underestimate hidden power__

More individual values are better except when a favorable type in hidden power is desirable as it can easily make up to missing points.

* __Night shade and seismic toss__

* __Rage is good against multi hit__

Each hit builds rage

## Combos

* __Beware of fake combos__
On average dynamic punch hits once every two turns, while the combo mind reader followed by dynamic punch guarantees to hit once every two turns. Not that great, especially considering that you are using an extra move slot and are more predictable; mind reader hints the opponent that something is coming.
* Mind reader + dynamic punch (just try dynamic punch twice)
* Sunny day + synthesis, morning sun or moonlight (just use a poyion instead)

* __List of combos__

Combos are multi turns and inherit all its disadvantages. Additionally remember to take into account the number of turns required to perform the combo when calculating values.
* Mean look + multi turn

* __Don't do dumb shit__

People just do it, like using rain dance and sunny day in one pokémon or same party, or trying to combo mean look with spikes.

They do it. But not you.

Avoid:
* Spikes + mean look
* Spikes + spider web
* Sunny day + rain Dance

# todo
The great question: What is the average number of turns in a battle? And for each pokémon?

* __Formulas__

$$hp = 10 + level \times \left( 1 + \frac{base + iv + \sqrt{\frac{ev}{64}}}{50} \right)$$
$$stat = 5 + level \times \left( \frac{base + iv + \sqrt{\frac{ev}{64}}}{50} \right)$$
$$damage = 2 + \frac{attack}{defense} \times \frac{power}{25} \times \left( 1 + \frac{level}{5} \right)$$

* __Test__

$$hp = damage$$

* __HM slaves__: are pokemons common, easy to catch and available relatively early game which are only there to use HMs for exploration. See https://pokemondb.net/gold-silver/hms
Personal recommendation: hoot-hoot (fly, flash), poliwag (surf, waterfall and whirlpool) and sandshrew (cut, rock smash, strenght). You may also consider headbutt

# List

- [ ] Absorb
- [ ] Acid
- [ ] Acid Armor +2
- [ ] Aeroblast
- [ ] Amnesia +2
- [ ] Ancientpower
- [ ] Attract
- [ ] Aurora Beam
- [ ] Barrage
- [ ] Barrier +2
- [ ] Baton Pass
- [ ] Beat Up
- [ ] Belly Drum +6
- [ ] Bide
- [ ] Bind
- [ ] Bite
- [ ] Blizzard
- [ ] Body Slam
- [ ] Bone Club
- [ ] Bone Rush
- [ ] Bonemerang
- [ ] Bubble
- [ ] Bubblebeam
- [x] Charm -2
- [ ] Clamp
- [ ] Comet Chop
- [ ] Comet Punch
- [ ] Confuse Ray
- [ ] Constrict
- [ ] Conversion
- [ ] Conversion 2
- [ ] Cotton Spore
- [ ] Counter
- [ ] Crabhammer
- [ ] Cross Chop
- [ ] Crunch
- [ ] Curse
- [ ] Cut
- [ ] Defend
- [x] ~Defense Curl~ +1 (except rollout combo)
- [ ] Destiny Bond
- [ ] Detect
- [ ] Dig
- [ ] Disable
- [ ] Dizzy Punch
- [ ] Double Edge
- [ ] Double Kick
- [ ] Double Slap
- [ ] Double Team
- [ ] Dragon Rage
- [ ] DragonBreath
- [ ] Dream Eater
- [ ] Drill Peck
- [ ] Dynamic Punch
- [ ] Earthquake
- [ ] Egg Bomb
- [ ] Ember
- [ ] Encore
- [ ] Endure
- [ ] Explosion
- [ ] Extreme Speed
- [ ] Faint Attack
- [ ] False Swipe
- [ ] Fire Blast
- [ ] Fire Punch
- [ ] Fire Spin
- [ ] Fissure
- [ ] Flail
- [ ] Flame Wheel
- [ ] Flamethrower
- [ ] Flash
- [ ] Fly
- [x] ~Focus Energy~
- [ ] Foresight
- [ ] Frustration
- [ ] Fury Attack
- [ ] Fury Swipes
- [ ] Future Sight
- [ ] Giga Drain
- [ ] Glare
- [x] Growl -1
- [x] Growth +1
- [ ] Guillotine
- [ ] Gust
- [ ] Harden
- [ ] Haze
- [ ] Headbutt
- [ ] Heal Bell
- [ ] Hi Jump Kick
- [ ] Hidden Power
- [ ] Horn Attack
- [ ] Horn Drill
- [ ] Hydro Pump
- [ ] Hyper Beam
- [ ] Hyper Fang
- [ ] Hypnosis
- [ ] Ice Beam
- [ ] Ice Punch
- [ ] Icy Wind
- [ ] Iron Tail
- [ ] Jump Kick
- [ ] Karate Chop
- [ ] Kinesis
- [ ] Leech Life
- [ ] Leech Seed
- [ ] Leer
- [ ] Lick
- [ ] Light Screen
- [ ] Lock On
- [ ] Lovely Kiss
- [ ] Low Kick
- [ ] Mach Punch
- [ ] Magnitude
- [ ] Mean Look
- [ ] Meditate
- [ ] Mega Drain
- [ ] Mega Horn
- [ ] Mega Kick
- [ ] Mega Punch
- [ ] Metal Claw
- [ ] Metronome
- [ ] Milk Drink
- [ ] Mimic
- [ ] Mind Reader
- [ ] Minimize
- [ ] Mirror Coat
- [ ] Mirror Move
- [ ] Mist
- [x] Moonlight
- [x] Morning Sun
- [ ] Mud Slap
- [ ] Night Shade
- [ ] Nightmare
- [ ] Octazooka
- [ ] Outrage
- [ ] Pain Split
- [ ] Payday
- [ ] Peck
- [ ] Perish Song
- [ ] Petal Dance
- [ ] Pin Missile
- [ ] Poison Gas
- [ ] Poison Powder
- [ ] Poison Sting
- [ ] Pound
- [ ] Powder Snow
- [ ] Present
- [ ] Psybeam
- [ ] Psych Up
- [ ] Psychic
- [ ] Psywave
- [ ] Pursuit
- [ ] Quick Attack
- [ ] Rage
- [ ] Rain Dance
- [ ] Rapid Spin
- [ ] Razor Leaf
- [ ] Razor Wind
- [ ] Recover
- [ ] Reflect
- [x] Rest
- [ ] Return
- [ ] Reversal
- [ ] Roar
- [ ] Rock Slide
- [ ] Rock Smash
- [ ] Rock Throw
- [ ] Rolling Kick
- [ ] Rollout
- [ ] Sacred Fire
- [ ] Safeguard
- [ ] Sand Attack
- [ ] Sandstorm
- [ ] Scary Face
- [ ] Scratch
- [ ] Screech
- [ ] Seismic Toss
- [ ] Selfdestruct
- [ ] Shadow Ball
- [ ] Sharpen
- [ ] Sing
- [ ] Sketch
- [ ] Skull Bash
- [ ] Sky Attack
- [ ] Slam
- [ ] Slash
- [ ] Sleep Powder
- [ ] Sleep Talk
- [ ] Sludge
- [ ] Sludge Bomb
- [ ] Smog
- [ ] Smokescreen
- [ ] Snore
- [ ] Softboiled
- [ ] Solar Beam
- [ ] Sonicboom
- [ ] Spark
- [ ] Spider Web
- [ ] Spike Cannon
- [ ] Spikes
- [ ] Spite
- [ ] Splash
- [ ] Spore
- [ ] Steel Wing
- [ ] Stomp
- [ ] Strength
- [ ] String Shot
- [ ] Struggle
- [ ] Stun Spore
- [ ] Submission
- [ ] Substitute
- [ ] Sunny Day
- [ ] Super Fang
- [ ] Supersonic
- [ ] Surf
- [ ] Swagger
- [ ] Sweet Kiss
- [ ] Sweet Scent
- [ ] Swift
- [ ] Swords Dance
- [x] Synthesis
- [ ] Tackle
- [ ] Tail Whip
- [ ] Take Down
- [ ] Teleport
- [ ] Thief
- [ ] Thrash
- [ ] Thunder
- [ ] Thunder Punch
- [ ] Thunderbolt
- [ ] Thundershock
- [ ] Thunderwave
- [ ] Toxic
- [ ] Transform
- [ ] Tri Attack
- [ ] Triple Kick
- [ ] Twineedle
- [ ] Twister
- [ ] Vice Grip
- [ ] Vine Whip
- [ ] Vital Throw
- [ ] Water Gun
- [ ] Waterfall
- [ ] Whirlpool
- [ ] Whirlwind
- [ ] Wing Attack
- [x] Withdraw
- [ ] Wrap
- [ ] Zap Cannon
