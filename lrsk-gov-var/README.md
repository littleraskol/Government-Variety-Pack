GOVERNMENT VARIETY PACK
A grab bag of new civics and government types.

1. New Civics

A total of 76 new civics, broken down into 10 origins, 22 normal civics, 19 hive civics, 14 machine civics, 14 megacorp civics, and 3 "advanced" civics available to any non-gestalt empire. Additionally, 3 base game civics have been enhanced with expanded features. All details are in this dedicated thread: https://steamcommunity.com/workshop/filedetails/discussion/2806903835/4839692156559653486/

2. New Governments

Around 85-90 new governments (I may have lost count at some point!) spread across nearly all authority types and combining vanilla and GVP-added civics. They are also listed in their own thread: https://steamcommunity.com/workshop/filedetails/discussion/2806903835/4839692156559694926/ (The requirements for making them are in the first reply to that thread.)

3. Known Issues

-In the base game, certain events (the Prethoryn and Unbidden crises, most critically) check to see if the player has certain set defined governments to determine what response to give. However, the default "OK" response doesn't start the crisis events. This means that if you're using any mod-added governments, it doesn't seem that you can start the crises. Fortunately, there is a mod out there that fixes this: Event Bugfixes by ECHO (http://steamcommunity.com/sharedfiles/filedetails/?id=785269836)

Report any issues you find here: https://airtable.com/shr57DnP3u6lzJ4D9

4. Compatibility

This mod only adds new things to the game, in new files. There's no possibility of this mod conflicting with another due to both editing base game files. All file names and tokens, furthermore, are specific to this mod (using a special prefix) so any token or file conflict would more or less have to be intentional (e.g. a patch or submod). That said, there's no guarantee that all the civic combinations between my mods and others will make sense or be balanced. Also, if a mod radically changes the way ethics work (especially renaming the base ethics), not all mod features can be guaranteed to be coherent.

5. Changes

v6.2.1 (9/13/24) - Post-Vela (3.13) Hotfixes
-Adjusted weights of GVP-added "criminal" governments so they override base game.
-Using scripted triggers to check authority in places that I missed.
-NPC fed partners now cannot be Xenophobes.
-Research Co-op Federation NPC origin was apparently preventing non-MI civics? Now prevents various MI civics the base game does not allow in federations.

v6.2.0 (9/10/24) - Vela (3.13) Update
-Fixed what was needed for compatibility with Stellaris 3.13 (Vela).
--Removed references to deprecated resource buildings (building_crystal_mines, building_mote_harvesters, and building_gas_extractors).
--Shifted pop growth from "Xenophobic" sources to use new founder_species_growth_mult modifier.
--Pass-through of inter-compatibility triggers (very technical).
-Updated compat version number.

v6.1.0 (7/19/24) - Built-In Adaptation to Ethics and Civics Classic
-Using random_weight and ai_weight to null out incompatibility between civics and E&C ethics to avoid randomly-generated and AI-player empires with silly combinations of ethics and civics.
-None of this will prevent players from making goofy combinations but whatever.

v6.0.7 (7/17/24) - Individual Machine Audit
There was more to do when it came to accounting for individualist machines and interactions with civics.
-Various backend tweaks (adding blocks_random_machine_empire_generation = yes as needed)
-Uplift Origin incompatible with individualism machines.
-Ascetic Virtues and Shroud Touched invalidated by synth ascension.
-Scientific Management replaced food usage reduction with housing and amenities usage reduction.

v6.0.6 (6/24/24) - Govt Weight Audit
-Came to my attention that the base game changed its weighting of governments so that base game governments outweigh those added by this mod where not expected. This should be fixed.

v6.0.5 (6/19/24) - wow
-supported_version now requires a 'v' incredibly important update

v6.0.4 (5/29/24) - Gestalt Civic Node Exp & Diplomatic Protocols Rework
-Gestalt civics are supposed to give exp gains to their nodes. The ones from this mod now do so.
-Diplomatic Protocols reworked into "Xeno Communication Expert System" (+10% first contact speed, +1 first contact clue, +1 first contact target difficulty, +10% trust growth, +10% trade attractiveness).

v6.0.3 (5/13/24) - Misc tweaks and fixes
-Just in case, made Shroud-Touched origin unable to be added after game start. (Modifies planet deposits, should always have been the case.)
-Moved setup event for Shapers/Artificers/Essentialists to the empire_init_add_technologies on_action trigger (in case it randomly spawns in game)
-Changed "Civic Leader" job name to "Civil Society Leader" and tweaked its description.

v6.0.2 (5/11/24) - Building Effect Reqs
-Several building types had no way of handling being owned by an empire without the originating civic. Now they do.
--Hall of Honor/Valor: Jobs only provided if owner has Chivalry.
--Synaptic buildings: Without Planetmind Creativity, only boosts soc research.

v6.0.1 (5/10/24) - Individualist Machines Hotfixes
-Shroud-Touched should not be available to individualist machines.
-Shapers should not be available to individualist machines.
-Ascetic Virtues should not be available to individualist machines.
-Utilitarian Planning now reduces pop housing and amenities usage (rather than food, for compatibility with individual machines)

v6.0 (5/7/24) - Andromeda (3.12) Update
-Fixed what was needed for compatibility with Stellaris 3.12 (Andromeda)
-Diplomatic Protocols deprecated (exists in base game now, same name and basic concept.)
-Added inline scripts to jobs for new automodding priorities.
-Updated compat version number.

v5.9.1 (4/25/24) - Filename Hotfix 
-Extremely embarassing filename error fixed.

v5.9 (2/27/24) - Eridanus (3.11) Update
-Fixed what was needed for compatibility with Stellaris 3.11 (Eridanus)
-Dealt with removed techs:
--Changed tech requirements for Artificers, Essentialists, and Shapers councilors.
--Reworked Uplift tutor empire creation to use base game advanced empire event to set techs (which I was also doing anyway...)
-Updated compat version number.

v5.8.1 (02/25/24) - Post Pyxis (or Pre-Eridanus?) Tweaks
-Republicanism effects changed to -20% Officials cost, +1 Officials cap, and 1 Civic Leader job per 25 pops. Civic Leaders are a specialist-level admin job. (Change made because adding ruler jobs per pop creates annoying unemployment issues as planet population fluctuates.)
-New governments for different ethics "flavors" of oligarchy/democracy with Republicanism.
-Renamed "Imperial Economy" civic to "Extractive Economy" (due to confusion related to Imperial authority name); this civic also no longer has strict authority limits but is unavailable to any Egalitarians.
-Renamed "Imperial Socialism" government to "Colonial Socialism" (due to confusion related to Imperial authority name) and reworded its description to match; this government also no longer has authority requirements. (Un-egalitarian social democracies can be colonialists too!)
-Removed most trait-based job logic (i.e., effects on output and chance of taking a job) and replaced them with the scripted calcs which the base game now uses.
-Overhauled Otherworld Guide job to be more dependent on psionic traits (and added concept text for this).
-Investigator and Suppressor are now more reliant on certain traits: 
--Psionic traits make the Investigator more effective (as a "legitimate" detective).
--Strength-based traits make the Suppressor more effective (as a goon sent to intimidate people).
-Fixed error where gestalt job was adding "regular" amenities (instead of the no-happiness version).
-Fixed various other bugs/errors.

v5.8 (11/17/23) - Pyxis (3.10) Update
-Fixed what was needed for compatibility with Stellaris 3.10 (Pyxis)
--Rework of Esper trait to match new multi-leader trait format (based on Psychic trait).
--Changed exp_gain modifiers to match new leader types (typically also added leader levels where appropriate).
--Changed leader_age to new leader_lifespan_add modifier.
--Generally substituted "official" for "governor" and "commander" for "admiral" and/or "general" as needed.
-Added missing localisation for "mod_councilor_ruler_imperial_exp_gain"
-Added new civic "War Profiteers" which is what now allows for the Military Excellence Academy branch office building (the Naval Contractors and Private Military Companies civics no longer provide this).
-Warrior Caste gets +1 Commander cap.
-Royal Caste gets +1 Official cap.

v5.7.2 (10/24/23) - Leader Levels -> Exp Gain
-MrFunEGUY helpfully pointed out that xxx_skill_levels modifiers are deprecated. They will be changed to xxx_exp_gain modifiers instead.
--Chivalry now gives +10% exp for admirals and generals.
--Lifelong Learning now gives +10% exp gain for scientists and governors.
--Warrior Caste now gives +10% exp for admirals and generals.
--Royal Caste now gives +20% exp gain for governors.
--Combat Data now gives +10% exp for admirals and generals.
--The "Deep Code: Profiling" trait from Uplift now gives -10% leader upkeep instead of +2 leader levels.

v5.7.1 (09/30/23) - Branch Office Building Concepts (& more!)
-Adding concepts for branch office buildings granted by corp civics.
-Altered casino luck random events so that when one happens, it's positive 80% of the time and negative 20% of the time (changed from 50%/50%).
-Tweaked some fixed opinion modifiers.

v5.7 (09/12/23) - Caelum (3.9) Update
-Fixed what was needed for compatibility with Stellaris 3.9 (Caelum)
-Updated compat version number.
-"Employee-Owned Co-op" civic renamed and reflavored due to introduction of the "Worker Cooperative" civic in base game.
--Renamed to "Labor Peace," flavor is more about labor/management compromise.
--"Organizing Hub" branch office building changed to "Labor-Management Retreat"
--"Employee Wellness Coordinator" councilor's flavor text modified somewhat to match new civic flavor.
--"Cooperative Enterprise" government now only available without Megacorp DLC.
--Shuffled around opinion modifiers to match.
-Supremacist Demagoguery now gives +1 max rivalries, +15% damage to rivals, +5% diplo weight from rivals, and +25% power projection.
-Because admin cap is back (in pog form), Planetmind Overseers now give +2 naval cap and reduce empire size by 2.
-Changed name of Universal Sovereignty councilor to "Client Obligations Guarantor"
-Backend: Replaced calls to base game "federation_origin_planet_setup" scripted effect with mod-added "lrsk_federation_origin_planet_setup" scripted effect that works the same way as the pre-3.9 scripted effect. (Base game version now works very differently, will take more effort to understand/adapt its new effects; the old way will work for now.)
-Various other backend things.

5.6.3 (05/23/23) - Republicanism Redux
-OR between authority and ethic does not work, so Republicanism is just going to be available to non-Authoritarian Oligarchies and (redundantly) Democracies.

5.6.2 (05/15/23) - Touching Up RRA
-Tweaked the odds in Run Recursive Analysis so the "worst" option is naturally the least likely (and all the base odds add up to 100...).
-Results of RRA now heavily factor in planet designations, and resource-related designations make bad outcomes much less likely.
-Player-facing descriptions make results and requirements more clear.
-The decision is overall more powerful in its ultimate results and less prone to bad outcomes, but costs more.
-Changed name and flavor of signature job.

5.6.1 (05/13/23) Post-Update Hotfixes
-Public Info Officer modifiers were all screwed up, now fixed.
-Vertical Integration's councilor shouldn't give the same benefit as the civic.
-Several other councilors had modifiers with the wrong sign, and so ended up being detrimental.
-Added "concepts" (sub-tooltips) to make tooltips less busy.
-Improved some old civic descriptions, and even some new councilor descriptions.

v5.6 (05/11/23) - Gemini (3.8) Update
-Fixed what was needed for compatibility with Stellaris 3.8 (Gemini)
-Updated compat version number.
-Added councilors for all non-gestalt civics.
-Civics have AI weighting by personality for in-game picks.
-Royal Proclamation of Justice now has an option for resetting policy cooldowns finally!
-"Crusader" governments can be enabled by Crusader Spirit civic.
--Crusader Kingdom: Crusader Spirit is an option along with Chivalry and Feudal Realm.
--Crusader Order: Either Chivalry or Crusader Spirit qualifies.
--Citizen Crusade: Being Spiritualist with Crusader Spirit is an option along with Exalted Priesthood and Elected Clergy.
--Crusading Company: Crusader Spirit is an option for the non-Megacorp implementation.
-RMF requires Precision Cogs.
-Military Excellence Academy now boosts general and admiral exp gain rather than directly assigning traits.
-Enlightened Liberalism now boosts Specialist political power by 50% and Worker political power by 25% (this one's for everyone who's commented on this civic being too dystopian, lol).
-Artificers now gets reduction of robot upkeep instead of increased robot production (benefit moved to councilor).
-Shapers now gets +1 organic species trait pick insteat of modification cost reduction (benefit moved to councilor).
-Ascetic Virtues now gets -1 leader negative traits and -10% food pop usage rather than a growth and leader age bonus (these benefits moved to councilor).
-Utilitarian Planning now gives +5% food production, +10% council agenda speed, -10% edict cost.
-Cult of Personality now gives -10% starbase influence cost instead of +5% influence production (benefit moved to councilor).
-Automated Indolence has been removed until I can figure out how to do something actually interesting with it.

v5.5.2 (4/19/23) - Better planet class detection (backend improvement)
-Can change the planet class to the ideal for species (in Uplift).
--This will enable better compatibility with mods adding new planet classes.

v5.5.1 (4/18/23) - Little weird "bug" "fix"
-There seems to be a base game bug in the random name parser that will cause it to read commented out text in localisation files. I have removed the comment that causes this specific issue, although the underlying problem may remain...

v5.5 (4/10/23) - Return of Better Names (and other updates)
-The "Better Names" feature returns thanks to the heroic efforts of Renan.
--This includes some (probably quite cack-handed) attempts at real localization for syntax functions.
-Other, unrelated changes:
--Royal Absolutism is incompatible with Feudal Society (because history).
--Automated World-Commune can be Oligarchic or Democratic.
--Local News Offices no longer engage in "Boradcasting" (and other typos finally fixed).
--Citizen Crusade requires either Exalted Priesthood or Elected Clergy (meaning it can be Democratic).
--Republican Directory requires either Enlightened Liberalism or Republicanism.
--Constitutional Plutocracy, Stakeholder Polity, and Proprietary Franchise now have actual female ruler titles for all you girlbosses out there.
--For some reason, changed the name of an Easter Egg government you can't get without modding in more than 3 ethic points. (Imperial Church of Slaughter is now Apocalyptic Theocracy.)
--Some backend tweaks only I care about.
-In an effort to make "subject-focused" civics more useful if you happen to not have subjects, the following civics get +15% diplomatic weight from the indicated source:
--Universal Sovereignty: Military
--Imperial Economy: Economy
--Exploitation Algorithms: Technology
--Benign Overmind: Pops
--Domineering Expectations: Empire Size

v5.4.2 (4/3/23) - Small fixes
-Safe system check needs to make sure owner exists before asking about it.
-Removed some redundant localization.

v5.4.1 (3/27/23) - Backend Cleanup and Inter-Compatibility
-Learned that a base game change apparently made to enable megacorps to be Galactic Emperor means OR logic between different categories of civic requirements is possible, resulting in the following:
--Deprecated duplicate variant of Chivalry for Aristocratic Elite (now able to make a civic require Imperial authority or Aristocratic Elite, removing duplicates).
--Deprecated duplicate variant of Republicanism for Egalitarian Oligarchies (now able to make a civic require Democratic authority or Egalitarian ethics, and the only non-Democratic Egalitarians are Oligarchies, removing duplicates).
--The deprecated civics still exist, but require themselves, and so can't be selected. An event should remove and replace them for any empires that have them.
-Added scripted triggers to check for each authority type, which enables other mods or patches to overload them with mod-added authorities.
-Government application logic now uses these scripted triggers rather than checking directly for authorities.
-Added scripted trigger (lrsk_gvp_is_active) to detect whether this mod is active/loaded (for other modders to check, basically...)

v5.4 (03/14/23) - Canis Minor (3.7) Update
-Fixed what was needed for compatibility with Stellaris 3.7 (Canis Minor)
-Updated compat version number.
-Supremacist Demagoguery now gives +10% damage to rivals instead of +30% army morale damage.
-Boundless Spite gives +1 max rivalries (reduced from +2) and +10% damage to rivals.
-Improved tooltips for Combat Data special events.

v5.3.9 (03/12/23) - Update prep
-Changes made to re-merge with master branch and prepare for 3.7
-Descriptions and documentation corrected (forgot to restore docs when features restored)
-Corp branch buildings have categories
-Removed spiritualist fed name fix (Paradox fixed)

v5.3.8 (02/28/23) - More bad (less boring) names
-Moved over more of the default name formats for added governments.
-Should be able to deal with "special" governments (e.g. purifiers) appropriately.
-Restoring "better names" from this mod is still a far off dream...

v5.3.7 (01/03/23) - Siege Mentality and Colonial Fief Fixes
-Siege Mentality now grants +10% home territory fire rate and +25% defense army morale instead of its previous defense platform build speed and damage bonuses.
--Slight localization tweak.
-Colonial Fief fixes:
--Random vassals should no longer start on Holy Worlds or in systems adjacent to Fallen Empires.
--Also they should have names...
-Some small backend changes.
-Fixed localization of Functionary job to show correct job effects.

v5.3.6 (12/13/22) - Little Things 2: The Ensmallening
-Removed redundant boxed-in escape route checks
-Colonial Fief spawned vassals were not copying techs from overlord.
-Small localization update.

v5.3.5 (12/12/22) - Little Things
-Forgot to add new origins to scripted triggers
-Wrong effects for NPC Convened by Providence

v5.3.4 (12/10/22) - Orion Post-Release Update 2
-Restored all federation start origins: the choice given by the new Common Ground does not guarantee any suitable fed partners the way my origins do, so that's positive value added. Plus, removing them broke custom empires for users.
-Added "Convened by Providence" origin to start player in a suitable Holy Covenant.
-Cleaned up new federation start code.
-Incidentally, fixed (most of the time) a base game error that prevents Holy Covenants from getting random names.

v5.3.3 (12/3/22) - Fix for (sigh) Imperial Economy
-The special service agreement terms should handle all effects, but the old modifier-based system was never removed. It has now been.
-Added localization description of effects of agreement terms (for some reason, term tooltips don't show any effects besides loyalty-per-month changes).
-Commercial agreements were way too powerful: market fee reduction per subject with commercial service is now -2%, down from -5% (did not realize it would just straight subtract that much from the fee!).
--This change has also been applied to Colonial Chartering special subjects, with a max reduction limit of -20%.

v5.3.2 (11/30/22) - Yet More Random Name Problems
-Hopefully adapted to the surprise new random name definition format.

v5.3.1 (11/29/22) - Orion Post-Release Update 1
-Restored "Diplomatic Directive: Discover" because Machine Intelligences cannot take Common Ground.

v5.3 (11/29/22) - Orion (3.6) Update
-Made custom pre-sapient (Uplift) traits 0-cost to match "Presapient traits now have no trait point or trait pick cost" in Orion.
-Deprecated the specialist federation origins - redundant with the changes to Common Ground, which gives a choice of type.

v5.2.1 (11/13/22) - Lithoid Upkeep Fix
-Planetmind Overseers should not have food upkeep for lithoids.

v5.2 (09/21/22) - Fornax Update
-Fixed what was needed for compatibility with Stellaris 3.5 (Fornax)
-Knight job renamed to "Cavalier" (avoids redundancy with new knightly origin in Toxoids)
-Did some improvements to Tradeways origins:
--Megacorp players should never have Megacorp fed partners.
--Merchant Guild players should have one Megacorp fed parter (small chance of 0 or 2).
-Imperial Economy returns (somewhat less dramatically):
--All benefits are based on a new subject agreement term unlocked by this civic, "Special Services," which provides the overlord four different benefits (with a penalty to the subject and loyalty hit).
--Special subject presets mostly set one of these Special Service options.
--Having at least one subject in a given service category provides a unique bonus.
-Planetmind Creativity rebalanced:
--Instead of -5% empire size from pops, civic grants -20% empire size from colonies and systems.
--Civic incompatible with Subsumed Will and Divided Attention (this is both a gameplay and thematic limitation).
--Upgrade costs of Synaptic buildings now scale more steeply (lower levels easier to get, higher level buildings harder to get).
--Planetmind Overseer job now gives naval cap instead of empire size reductions (there's just no way to balance scaling percentages, RIP admin cap) and reduces housing usage on planet by 10%, while having a unity upkeep instead of an energy upkeep. Influence production reduced to +0.1, crime added reduced to 5.
--This is a work in progress and feedback welcome. Not using empire size mods on the job frees up more room to tinker because they can scale properly now.

v5.1.4 (09/08/22) - Minor Fixes
-CWTools flagged errors: deprecated/changed diplo blocks, incorrect preset keys, missing locs.
-Reactionary Socialism lacked an hier title.

v5.1.3 (07/07/22) - Imperial Economy Deprecated
-Due to a bizarre base game bug involving agreement terms, the core features of the Imperial Economy civic prevent subject taxes from being collected. It has been removed until this is fixed.

v5.1.2 (06/20/22) - Return of Fixed/Updated/Adapted/Imrpoved Imperial Economy & Chartered Colonies
-See v5.1 changelog entry for overall list of changes.
-Only difference is the lack of "fine tuning" for Imperial Economy. This requires the ability to limit who can see resource sliders with conditions in a potential = {} block, but for some reason if I add such a slider, it prevents anyone from changing agreement terms. For now the special subject resource taxes come from hidden resource sliders.
-Known issue (minor): When leaving the Chartered Company preset, the empire is supposed to have its government restored from before it was changed into that type of vassal (which comes with a change in government). This does not seem to be working? Not the end of the world, kind of an edge case, but hopefully will be fixed in the future.

v5.1.1 (06/12/22) - Adding Special Subject icons
-Icons for added subject types.

v5.1 (06/12/22) - Fixed/Updated/Adapted/Imrpoved Imperial Economy & Chartered Colonies
-Specialized subjects for both civics can still be added by event, but change from the Agreement menu is supported.
-Imperial Economy allows for "fine tuning" subject resource contributions: You can individually set the taxes or subsidies of each resource type.
-Changed the way the Imperial Economy special vassals work:
--Taxes are based on setting agreement minimums, not preset definitions.
--Each special type provdes a special bonus to the overlord (tied to innate loyalty penalty).
--Foundry Colony renamed to Logistics Colony (more accurate to purpose).
--Logistics Colonies Taxed 15% of alloys and energy.
--Market Colonies Taxed 15% of consumer goods and food.
--Prospecting Colony renamed to Provisioner Colony (Overlord DLC has a "Prospectorium" specialized subject).
--Provisioner Colony Taxed 15% of minerals and strategic resources.
--Trophy Colony Taxed 15% of unity and influence.
--No limits on how many of these vassals one can have.
--Bonus for each reduced to +1 stability from +2.
--Special subject status can be changed after setting (using Agreement menu).
-Chartered Colony subject type changes:
--Taxed 15% of Basic Resources.
--Innate trust (opinion bonus) in chartering overlord reduced to +25 and +25 (decaying) from +100.
--Halved "Divided Loyalties" penalty for this subject type.
--Innate loyalty bonus (tied to small Trade Value bonus for subject).
--Choosing to install your species as rulers will benefit xenophobes and authoritarians, and increase subject monthly loyalty, but may lead to general unrest in the subject.
--Improved process for "foreign rule" option, no longer completely destroys and replaces government, just changes primary species (and a few other things).
--Greatly increased the "Colonial Trade" modifier bonus, making it the major benefit.
--Updated effect description.
--Subject status can be changed after setting (using Agreement menu).
--Previous government should be restored if colonial charter ended.
-Removed various logging outputs.

v5.0.4 (06/01/22) - Trying to fix "code names"
-The only difference between my name generators and Paradox's are the quotation marks I had around the format string. So I removed them. Hope this helps!

v5.0.3 (05/28/22) - Localization Updates
-Providing new (missing) localizations for subjects.

v5.0.2 (05/15/22) - Yet More Post-Release Fixes
-Explorer Colonies spawned by Colonial Fiefs empires get a resource boost based on the game year to make them viable (got reports that they collapsed due to not having any unity).
-Fixed lookups to work around possible bug causing %ADJECTIVE% adjectives for empires. (Thanks MaskofKeter!)

v5.0.1 (05/12/22) - Post-Release Fixes
-Removed unneeded warning for Uplift (it uses standard presets).
-Fixed more lozalization format issues.
-Updating documentation.

v5.0 (05-12-22) - Cepheus Update
-Fixed what was needed for compatibility with Stellaris 3.4 (Cepheus)
-Updated compat version number.
-Fixed misc things for new version.
-Adapted branch buildings to new holding system.
-Uplift no longer requires any DLC... (This was pure oversight on my part.)
-Changed specialized vassals into "presets".
-Added warning about special vassal civics not working well yet.

v4.2 (03-25-22) - New Origin & Colonial Chartering Civic
-Added new origin: Uplift lets you play as the subject of an uplift/enlightenment action, starting as a special vassal of an advanced start empire that raised you to the stars. You have the option to select special species traits or an empire bonus.
-New megacorp civic Colonial Chartering: +15% research and mining station output, special vassal interactions (ht to Garlic Pudding for inspiration) - intended to replicate the European "colonial companies" of the Early Modern Era.
-Added new government type "Colonial Charter Board" based on the above civic.
-Changed Functionary job to produce unity instead of giving empire size penalty reductions, making it more like a mini Clerk/Bureaucrat hybrid (which was its original design idea).
-Fixed minor random name error. ("Failed to find part list 'lrsk_schl_type' in name random names lists")

v4.1 (03-22-22) - Balance Pass 2
-Citizen Scholar pops produce +2 amenities and +1 research if they have the Utopian Abundance living standard. (This is so that it's not strictly worse to be in this job than unemployed.)
-Planetmind Creativity requires some work given the new game systems. With unity being more useful for more things now, its Planetmind Synapse buildings' unity cost and upkeep hurt a lot more. So I'm making the jobs it gives cost less and give more and something more impactful and not granted by other civics or by APs.
--Planetmind Creativity now grants a flat -5% to empire size from pops rather than -15% housing usage.
--Planetmind Overseers now grant -1% empire size from pops rather than -1% empire size from colonies.
--Planetmind Overseers now grant -2% pop housing usage.
--Planetmind Overseers influence production increased to 0.2 from 0.1 (influence matters less).
--Planetmind Overseer crime addition reduced to 10 from 15.
--Planetmind Overseer stability loss reduced to 1 from 2.
--Planetmind Overseer food and energy upkeep reduced to 2 from 3.
-Jobs-per-pop modifiers are in a worse place since the game was rebalanced to reduce the number of pops overall. Therefore, the number of such jobs added by various sources has generally been doubled.
--Builder Caste now grants one Maintenance Drone per 10 pops, up from 1 per 20 pops.
--Warrior Caste now grants one Warrior Drone per 15 pops, up from 1 per 30 pops.
--Royal Caste now grants one Synapse Drone per 20 pops, up from 1 per 40 pops.
--Elected Clergy now grants one Pastor per 20 pops, up from 1 per 40 pops.
--Republicanism now grants one Politician per 25 pops, up from 1 per 50 pops.
--Direct Revelation now grants one Hedge Preacher per 15 pops, up from 1 per 25 pops.
--Shroud Pockets deposit grants one Otherworld Guide per 25 pops, up from 1 per 40 pops.
--Promote Citizen Scholarship edict grants one Citizen Scholar per 15 pops, up from 1 per 25 pops.
-With unity being a more useful and more widely used resource, jobs producing unity should produce more of it to make it a useful bonus.
--Pastors produce produce 5 unity, up from 3.
--Hedge Preachers produce 4 unity, up from 2.
--Otherworld Guides produce 2 unity base, up from 1. Trait bonuses unchanged.
--Regional Coordinators produce 9 unity, up from 6.

v4.0.6 (03-19-22) - Balance Pass 1
-Shapers, Artificers, and Essentialists civics now only give -5% researcher job output, rather than -10% overall research output, in their non-favored areas.
-Shapers no longer gives a growth bonus.
-Artificers robot job output bonus down to +5%, from +10%

v4.0.5 (03-19-22) - Fixes Continued 4
-Fixed issue preventing governments that adopt Colonial Fiefs mid-game from being able to change their Explorer Colonies policy.

v4.0.4 (03-11-22) - Fixes Continued 3
-Work Allocation Plan should not be infinitely stackable.

v4.0.3 (03-11-22) - Annoying Fix 2
-Esper rulers should not give +115% unity production.

v4.0.2 (03-10-22) - Annoying Fix
-Personal Protection Office was giving the wrong ethics attraction.

v4.0.1 (03-05-22) - Libra Cleanup
-Fixed some localizations.
-Various documentation updates.
-Various backend changes.

v4.0 (02-25-22) - Libra Update
-Various internal changes to adapt to Stellaris 3.3 (Libra).
-Royal Absolutism civic now gives +30 Edict Fund and -10% Edict Cost instead of +1 Edict Cap.
-The "Chancellor" option in the "Proclamation of Justice" event gives a unity reward as well.
-The "Estates General" modifier (from the Royal Absolutism special Edict) now gives +100% Edict Fund mult instead of +1 Edict Cap.
-The "Promote Citizen Scholarship" Edict for Lifelong Learning now costs 20 Unity upkeep.
-Supremacist Demagoguery and Boundless Spite civics now give +25% power projection.
-Reciprocal Planning Routines civic gives -10% Empire Size from systems, -20% Empire Size from planets, and -15% Empire Size from districts rather than +20 admin cap.
-Various effects related to influence have either been replaced with unity or augmented with unity.
-Everything modifying admin cap has been replaced with modifiers to the effects of empire size.

v3.3.1.5 (01-27-22) - All out of joke names at this point tbh
-Added tooltips of special effects to Combat Data and Imperial Economy.
-Improved the Universal Sovereignty tooltip.

v3.3.1.4 (12-31-21) - Backend Fixes/Updates Part 4 -The Fixes Resurrection
-Variable-multiplier-based modifiers were not working as intended.
-Happy New Year!

v3.3.1.3 (12-12-21) - Backend Fixes/Updates Part 3 - This Time It's Super Annoying
-Can't believe I missed a bunch of governments that lacked election candidate blocks and outgoing ruler definitions!!!
-Actually I can believe it.....................

v3.3.1.2 (12-10-21) - Small improvement
-Explainers now have a delay.
-Some small degree of process efficiency.

v3.3.1.1 (12-10-21) - Backend Fixes/Updates (continued...)
-Missed some election weights!!!

v3.3.1 (12-10-21) - Backend Fixes/Updates
-Colonial Fiefs has special effect tooltip.
-Changed some localization to use keys rather than user-facing text.
-Created NPC namelist so "Lesser Names Patch" won't let NPC-only govs go nameless.
-Democratic and Oligarchic initial rulers that get voted out should have a leader class to change careers into rather than vanishing (so long as this feature works...)
-Revised election weights in all electoral governments to have more vanilla values (some were downright weird).

v3.3 (12-05-21) - Civic Improvements 4
-Colonial Fiefs now has a policy that allows for pops to migrate and start new vassal empires.
-Added three new "advanced" mutually-exclusive and antagonistic starting-only civics focused on the idea of cultures that specialized in different domains of knowledge. Any non-gestalt empire can start with them.
-New Civic: Shapers (+5 leader age, -10% genetic modification cost, +10% habitability, +10% growth, -10% non-society research, start with "Eco Simulation" tech.)
-New Civic: Artificers (-10% ship build cost, -10% planetary structure build cost, +10% robot output, +10% robot build speed, -10% non-engineering research, start with "Powered Exoskeletons" tech.)
-New Civic: Essentialists (+10% ship and planet sensor range, -10% FTL windup and winddown time, -10% non-physics research, start with "Fusion Power" tech.)

v3.2.1.1 (11-27-21) - "Cosmic" Empires fix
-The re-instated "galactic" governments never got their names back...

v3.2.1 (11-27-21) - Herbert Update
-Fixed job calculations for compatibility with Stellaris 3.2.* (Herbert)
-Changed compat version number.

v3.2 (10-07-21) - Civic Improvements 3
-Imperial Economy is allowed to change vassals into specialized subjects.
-Minor fix: Sanity checks for 'esper' traits only being called every 2 years, every year preferable.

v3.1 (09-28-21) - Civic Improvements 2
-Combat Data now has a chance to improve military intel on an empire after the end of a space battle with that empire.
-Fixed an issue where mod-added branch office buildings were not useful for criminal syndicate empires. Now all branch office buildings added by this mod will give a flat +20 crime for criminal syndicates. This is balanced by legit megacorps having a better "normal" bonus.
-Royal Justice event option cost change: Ennobling officials costs 300 consumer goods per "established" (more than 2 pops, no Colony Shelter) colony.
-Royal Justice event option cost change: The Assembly of the Estates costs 20 energy per free pop in the empire.
-Royal Justice event option reward change: "My chancellor will tell you the rest..." gives reward as a multiple of influence production.
-Fixed a documentation and localization typos.

v3.0 (09-14-21) - Lem Update
-Fixed what was needed for compatibility with Stellaris 3.1.* (Lem)
-Changed compat version number.

v2.2 (09-11-21) - Civic Improvements 1
-Lifelong Learning: Gets access to the Promote Citizen Scholarship edict that gives special researcher jobs per pop.
-Utilitarian Planning: Gets access to the Work Allocation Plan planetary decision, which alleviates unemployment.
-Royal Absolutism: Gets access to the Proclamation of Justice edict that gives the player a choice of different effects on empire governance.
-Imperial Economy: Incompatible with Fanatical Purifiers and Inward Perfection.
-Direct Revelation: Now has options to ignore Wild Cult popups.
-Direct Revelation + Doomsday origin special modifier reduced in effectiveness to 20% from 25%.
-Using new modifier multipliers, the Offworld Worker bonus now scales without limit.
-Universal Sovereignty: Gets an opinion boost with weaker independent empires.
-Universal Sovereignty incompatible with Supremacist Demagoguery.
-Various civic combinations have triggered diplomatic opinion modifiers.
-New federation origins: Copied over trust and intel boosts from base game.
-Returned the "Galactic Empire" joke governments under new, even more bombastic names.
-Pure Social Republic government: renamed Purity Collective.
-Improved logic for finding "escape routes" for origins that start with nearby AI players.
-Bugfix: Technocracy prefix_formats used wrong part key.
-Various other small improvements and fixes.

v2.1.2 (06-06-21) - Localization Hotfix
-Fixed incorrect localization in a "casino luck" event (tourism bonus).

v2.1.1 (04-19-21) - Spy Stuff
-Investigation & Security Services gets +1 Encryption and Codebreaking, crime mult reduction down to -10% from -15%.
-Siege Mentality gets +1 Encryption instead of +5% station hull points
-Siege Mentality gets -20% military platform build cost (doubled from -10%)

v2.1 (04-18-21) - Dick Expansion (lol)
-Supremacist Demagoguery: Now gets +30% army morale damage (up from +20%).
-Combat Data: Now gets +30% army morale damage (up from +20%).
-Boundless Spite: Now gets +50% purge speed.
-Gestalt Extroversion: Now gets +10% first contact speed instead of +20 trust cap.
-Diplomatic Protocols: Now gets +1 first contact clues instead of +10% trust growth.
-Megacorp civics now available with Galactic Soveriegn civic.
-Removed now thematically redundant "galactic empire" govtypes.

v2.0 (04-18-21) - Dick Update
-Fixed what was needed for compatibility with Stellaris 3.* (Dick)
-Changed compat version number.
-Going forward, mod version numbers will change the major number with each Stellaris update that wrecks backwards compatibility (i.e. actual good version numbering practice)
-Some fixes to localization fixes.
-Enlightened Liberalism is not compatible with Shared Burdens.

v1.6.8.2 (01-14-21) - Misc fixes
-Removed defunct diplo phrase.
-Misnamed planet modifier (DPS building focus should now work)
-AI chances for options in events needed factors, not additions.

v1.6.8.1 (01-08-21) - New features and fixes
-Added option for media corp favor events: corp can bail out with no effect if desired.
-Fix: Incorrectly marked Braz/Port localization as French.

v1.6.8 (01-01-21) - Megacorp Expansion
-Scientific Management civic now allows the Managerial Technique Institute branch building, which provides the host planet with two Functionary jobs (produces +3 admin cap and +3 trade value) and provides the megacorp with +10% Branch Office Value, +5% more per Functionary job filled (which becomes +10% crime on planet per job for criminal corps).
-Educational Consortium civic now allows the Learnarium Dome branch building, which provides the host planet with +50% Materialist attraction and two Info-Guide jobs (produces +2 all research and +2 amenities), and provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Materialist.
-Employee-Owned Co-op civic now allows the Organizing Hub branch building, which provides the host planet with +50% Egalitarian attraction, +20% Worker power, and +10% Worker happiness, and provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Egalitarian.
-Gig Economics civic now allows the Odd Jobs Emporium branch building, which provides the host planet with two Gofer jobs (produces +4 amenities and +2 consumer goods), and provides the megacorp with +10% Branch Office Value, +5% more per Gofer job filled (which becomes +10% crime on planet per job for criminal corps).
-Naval Contractors and Private Military Companies civics now allow the Military Excellence Academy branch building, which provides the host planet with +50% Militarist attraction, the host empire with an improved chance of military leaders gaining positive traits, and provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Militarist.
-Indentured Assets civic now allows the Reformatory Workhouse branch building, which provides the host planet with +10% worker/slave output, and provides the megacorp with +15% Branch Office Value. Criminal megacorps with this building occasionally steal and enslave pops from the planet!
-Private Prospectors civic now allows the Offworld Jobs Placement branch building, which provides the host planet with two Offworld Worker jobs (produces +4 trade value and +2 energy), and provides the megacorp with improved colony growth speed and station output, and +5% Branch Office Value per Offworld Worker job filled (which becomes +10% crime on planet per job for criminal corps).
-Media Conglomerate civic now allows the Local News Office branch building, which provides the host planet with +10% ruler output, +20% specialist political power, and +5% specialist happiness. It provides the megacorp with a chance to occasionally get favors from the host empire.
-New Casino Mysticism civic (Not Materialist) provides -25% pop demotion time, +25% colony development speed, and allows the Grand Casino branch building, which provides the host planet with +10 amenities and +5% trade value, while enabling random beneficial and detrimental events for both the planet and the corp. It provides the megacorp with either +10% Branch Office Value or adds +15% crime (for criminal corps).
-New Vacation Experience Planning civic (Xenophile) provides -10% pop amenities usage, and allows the Galactic Excursions Office branch building, which provides the host planet with +50% Xenophile attraction and -15% pop amenities usage, and provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Xenophile.
-New Heritage Trust civic (Xenophobe) provides +5 stability, and allows the Heritage Museum branch building, which provides the host planet with +50% Xenophobe attraction and +10% citizen pop happiness, and provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Xenophobe.
-New Conflict Resolution Specialists civic (Pacifist) provides +15% trust growth rate and +20 trust cap, and allows the Mediation Retreat branch building, which provides the host planet with +50% Pacifist attraction and +5 Stability, and provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Pacifist.
-New Investigation & Security Services civic (Authoritarian) provides -15% crime, and allows the Professional Protection Office branch building, which provides the megacorp with increased Branch Office Value that scales with the proportion of the planetary population that is Authoritarian. The host planet gets +50% Authoritarian attraction and either an Investigator job (produces -25 crime, -15% Worker power) or (if the providing corp is criminal) a Suppressor job (produces -25% Worker power, +10% Worker output).
-New governments Private Intelligence Agency (Investigation & Security Services) and Protection Racket (Investigation & Security Services with Criminal Heritage).
-Every non-ethics based new branch office building has a different bonus for criminal empires.
-Update: Due to addition of "death cult" themed things to the game w/ the Necroids pack, changed "Death Cult" government to be named "Church of Slaughter"
-Employee-Owned Co-op civic no longer has civic restrictions (neither do any other ethos-special civics, afterall).
-Backend: Added "general test" diagnostic event.
-Backend: Numerous testing tools in scripted effects/triggers.
-Fixed some localization typos here and there.

v1.6.7 (11-11-20) - More Merchantry
-Added two governments based on the ideas of Steam user Garlic Pudding: Stakeholder Polity and Shareholder Commonwealth.
-Added new governments: Merchant Republic and Constitutional Plutocracy.
-Republicanism now available to Egalitarian Oligarchies.
-Institutionalized Collectivism incompatible with Merchant Guilds.
-Educational Consortium requires some degree of Materialist.
-Updated documentation.
-Fix: Porting localization that had been neglected.

v1.6.6.3 (11-10-20) - Minor format fix.
-The Entrepreneurial Council government lacked a valid female ruler title, was overriding the Enterprise Society female ruler title.

v1.6.6.2 (11-08-20) - New Fed Start Tuneup, Other Housekeeping
-Added scripted triggers to simplify checks for Research Fed and Trade Fed origins.
-Better companion empire generation for Trade Fed origins.
-Added NPC version of Tradways, Inc.
-Fixed companion empire gen to add correct NPC origins.
-Added scripted triggers to detect whether an empire is using mod-added content.
-Addressed vanilla issue where Common Ground and Hegemon origins can't always match custom empires with federation mate ethics.
-Fixed democratic Cosmic Choir lacking a Xenophile requirement option.
-Removed redundant backend check for empire starts that might lack sufficient exploration avenues (was called twice).
-Minor tweak to fed start colony detection (1 guaranteed habitable no longer overlaps with 2 or more).
-Randomly spawned Rogue Servitor federation mates had bugged pops that I could not fix (i.e., machine bio trophies) so I removed them...
-Enlightened Liberalism not compatible with either Workers' Councils or Institutionalized Collectivism.
-Updated compat version number to 2.8 (Butler) - could not verify any reports of incompatibility.

v1.6.6 (07-20-20) - Minor New Content and Feature Improvements
-This update ports over some smaller improvements and pieces of new content from the future version 1.7, because other content in that version is extensive and requires a great deal of testing. I don't want to wait on releasing this much less intensive stuff.
-New megacorp civic Gig Economics: -25% pop resettlement cost, +5% ruler and specialist happiness.
-New megacorp civic Controlling Interest: -75% election influence cost, -5% Market Fee.
-New megacorp civic Vertical Integration: +5% Energy and Mineral production, +5% Trade Value
-New megacorp civic Employee-Owned Co-op: Increased production and political power of workers and specialists.
-Added some origin icons.
-Added two government types (more to come) based on the ideas of Steam user Garlic Pudding, Crusading Company and Merchant Principality (see original post here: https://steamcommunity.com/workshop/filedetails/discussion/901988941/1318835718938058107/ ).
-Civic Budgetary Thrift now also provides -5% Market Fee.
-Civic Hoarder now also provides +7500 mineral storage.
-Civic Self-Aware Production Targets now also provides +2.5% alloy production.
-Civic Direct Revelation now has special interactions with the "Doomsday" Origin and a grace period at game start.
-New government type Citizen Crusade: Combination of Citizen Service and Exalted Priesthood.
-New government type Cooperative Enterprise: Corporate authority and Employee-Owned Co-op OR Corporate Dominion and Workers' Councils.
-Government Market Socialism now only a combination of Merchant Guilds and Workers' Councils.
-Two government types renamed (Social Imperialism -> Imperial Socialism, Socialism In One State -> Exemplary Socialism).
-Fix: Added election weights to some governments missing them.
-Fix: Minor change to Warrior Caste jobs-per-pop to bring more in line with intent.
-Fix: Shroud Touched trait marked as improving leaders.
-Balance: Removed "trollish" lack of empire cluster restriction on Galactic Backdoor (due to how this might affect players using other origins if this origin spawns randomly for an AI empire...)
-Tweak: Improved hyperlane logic for origins that have nearby other empires.
-Tweak: Slight improvements/additions to name gen.
-GFX: Included graphic for Run Recursive Audit decision.
-GFX: Changed the preview image for Grand Alliance.

v1.6.5.1 (07-17-20) - QCC, SC Fix
-Fixed localization of Quasi-Collective Consciousness diplo lines.
-Removed unused diplo prompts/actions, added new.
-Added "Simple Chinese" synced localization file for empire formats.

v1.6.5 (05-12-20) - Wells Update
-Royal Absolutism now also gives +1 Edict Cap.
-Business Lobby has become "Budgetary Thrift" and will be reworked into something more interesting (hopefully) in a future update, but Merchant Guilds just makes it thematically redundant.
-Workers' Councils not incompatible with Budgetary Thrift.
-Corporate Neofeudalism now requires Merchant Guilds instead of Business Lobby.
-Galactic Cartel (non-Megacorp version) now requires Cutthroat Politics or Shadow Council instead of Business Lobby.
-Proprietary Franchise now requires Cutthroat Politics rather than a choice of that or Business Lobby.
-Changed compatible version number to 2.7.*

v1.6.4 (04-16-20) - Small fixes and improvements
-Added icons for Educational Consortium, Scientific Management, and all new origins.
-Fix: Natural Esper costs no trait points (this prevented players using the Shroud-Touched origin from selecting as many species traits as should be possible).
-Fix: Ported over logic to prevent origins that spawn nearby AI-controlled systems from being boxed in.
-Fix: Grand Alliances should not spawn after game start...
-Fix: Agrarian Monarchy start screen message should display.

v1.6.3 (03-26-20) - Deposit hotfix attempt 2
-Added a checkup event to add back any planet deposits that might be removed by other mods.

v1.6.2 (03-25-20) - Deposit hotfix attempt 1
-Fixing possible compatibility issue: Otherworld Pocket deposit define might have conflicted needlessly with planet mods. Hopefully not anymore!

v1.6.1 (03-24-20) - Namazuo Governments
-Added 16 new governments, based on the ideas of Steam user Namazuo "Horse Poop" Toushiro posted here: https://steamcommunity.com/workshop/filedetails/discussion/901988941/1318835718938058107/ (only took two years...)
-Government type Proprietary Franchise now requires Merchant Guilds and either Business Lobby or Cutthroat Politics.
-New government type Empire of Rapine (Barbaric Despoilers and Enlightened Liberalism, Imperial authority ).
-New government types Agrarian Social State and Agrarian Commonwealth (Institutionalized Collectivism and Agrarian Idyll, Oligarchic or Democratic authority, respectively).
-Added special name gen for Xenophile Citizen Service govs (might be more about an interstellar army's glory or somesuch)
-Documentation: Diplo Protocols descriptions include actual benefits.
-Bugfix: Esper trait correctly shows that it improves leaders.
-Backend: Tweaks to Better Names gen.

v1.6 (03-21-20) - Origins
-Added seven new origins.
-Galactic Backdoor is like Galactic Doorstep, but with a wormhole instead of a gateway. (Not as sophisticated in terms of special event support yet.)
-Shroud-Touched is intended to be a "psionic" counterpart to the Syncretic Evolution and Mechanist origins, starting you down the path of the psionic ascension part-way.
-For Discovery and Diplomatic Directive: Discover both start you as leader of a Research Co-op, but the latter is for Machine Intelligences.
-Tradeways and Tradeways, Inc. both start you as leader of a Trade League, but the latter is for Megacorporations.
-Grand Alliance starts you as leader of a Martial Alliance.
-The machine civic Diplomatic Protocols is now more in line with the base game diplomatic civics, providing an extra Envoy and a minor diplo weight buff (the other modifiers remain but some have been nerfed).
-Job definitions now include "possible_pre_triggers" as seems to be needed now?
-Bug fix: Moved army morale bonus in knight building to army modifiers section.
-Bug fix: Added missing "add job" icons for some custom jobs.
-Documentation: Added the "Cooperative Super-Sapience" info to the government thread.

v1.5 (03-18-20) - Distributed Planning Systems Overhaul, Real Verne Updates
-Distributed Planning Systems maintains its base bonus but now also allows for a new planet decision. This decision, "Run Recursive Audit," temporarily adds jobs with a mix of beneficial and problematic effects. After a year, the "audit" ends and a longer-term modifier to planet output is applied. The more specialized a planet is, the higher the likelihood of a beneficial outcome.
-Elected Clergy now gives +10% faction influence instead of +0.5 max faction influence (defunct modifier).
-Universal Sovereignty now reduces subject integration cost by 25% (removed integration cooldown, not clear it even works or is that useful).
-Analgesic Stoicism changed to "Toiling Multitudes" and increases simple drone output instead of habitability because Ascetic now increases habitability (and was conceptually overlapping anyway).
-Planetmind Creativity changed base bonus to -15% housing usage, as Ascetic now reduces amenities usage.
-Backend: Further consolidation of localization files (civics and governments now in one file).

v1.4.10 (03-17-20) - Verne Updates
-Changed version number.

v1.4.9 (01-12-20) - Planetmind Creativity Overhaul
-Planetmind Creativity now allows Planetary Synapse buildings that improve amenities production, compound deviancy, and add Planetmind Overseer jobs.
-Planetmind Overseers produce small amounts of influence and increase empire admin cap, but reduce planet stability and increase deviancy.
-Added new government "Cooperative Super-Sapience" to reflect hive minds with Planetmind Creativity as something like a "committee" of collective minds with one presiding over the others.
-Small fix: updated version number in descriptor.mod

v1.4.8 (11-23-19) - Direct Revelation Rebalance, Megacorp Additions and "Restorations"
-Wild Cult formation is now assessed per planet, which is a better form of scaling than previous "more planets = more cult formation chance" method.
-Each cult on a planet decreases the likelihood of a new cult forming there.
-Wild Cult ethos attraction modifiers buffed.
-Wild Cults now only give one Hedge Preacher job (down from two).
-New Wild Cult added: "Wild Revelry Cult" (increase happiness but also crime, more ethos shift).
-New Wild Cult added: "Penance and Redemption Cult" (decrease crime but also happiness, less ethos shift).
-New Megacorp civic: Scientific Management (Not Egalitarian) - This business grew through precise and empirically tested management techniques that govern every aspect of employee life: the tools, workspaces, physical motions, work rhythm, on and off the clock, from cradle to grave. (-10% pop food requirements, +10% worker production output)
-New Megacorp civic: Educational Consortium (None) - This conglomerate specializes in providing high-quality edu-info-tainment product-experiences to expand the minds of customer-pupils young and old. (+10% specialist production output, +20% leader experience gain)
-Innovation Initiative and Rationalist Managerial Firm governments return to Megacorp DLC users based on these civics.
-Market Socialism now requires Workers' Councils and either Corporate Dominion or Merchant Guilds.
-Backend: Merged start screen messages to be with their associated government descriptions.
-Backend: Moved personality/diplomacy to "other" text definitions.
-Backend: Deleted "lrsk_gov_var_start_screens" and "lrsk_gov_var_personalities" files (text moved elsewhere).
-Removed some typos and such.

v1.4.7 (11-03-19)
-Better job descriptions.
-Cleaned up building definitions.
-Changed compat version to 2.5.*

v1.4.6.3 (10-19-19)
-Added global mod flag.
-Fixed some descriptions.

v1.4.6.2 (01-05-19)
-Fixed an issue with diplomatic phrases (some clauses now not in use?).
-Fixed misc issues.

v1.4.6.1 (01-01-19)
-Added simplified Chinese localization.
-Fixed incorrect job provision (Elected Clergy are no longer fanatical hedge preachers...)

v1.4.6 (12-31-18) - Balance Audit
-Elected Clergy: Changed edict duration bonus to +1 Pastor jobs per 40 pops.
-Added new Pastor job: Specialist, like a Priest but consumes one less Consumer Goods and provides no Society Research. (Only provided by Elected Clergy civic effect.)
-Ascetic Virtues: Buffed to provide +15 years to leader age (was +10).
-Republicanism: Buffed to provide -30% leader cost (was -20%).
-Republicanism: Changed leader pool buff to +1 Administrator jobs per 50 pops.
-Utilitarian Planning: Reduced to provide -5% pop food requirements (was -10%, which is equivalent to a tradition opener all on its own).
-Utilitarian Planning: Removed -15% resettlement cost (Corvee System civic already does this, and it's quite strong).
-Universal Sovereignty: Fixed tooltip (has erroneously shown the integration time reduction as a red malus forever, this is the base game doing something weird, but I have 100% verified reduces the integration time as desired (also nothing uses this in the base game anymore so will it last...??)).
-Enlightened Liberalism, Void Affinity, and Astro-Prospecting Mainframe: Doubled both bonuses to +20% (have heard station output is weak as it stands).
-Knight job: Overall reduction in crime suppression (some conditions improve this bonus).
-Lifelong Learning: Buffed to provide +20% leader experience gain (was +15%, this modifier for civics using it tends to be only +10% and paired with a +1 boost to all leader skill levels rather than just some).
-Colonial Fiefs, Unending Bloom, and Optimized Expansion: Nerfed to provide -5% starbase influence cost (was -10%, this is equivalent to a tradition right out the starting gate on top of the colonization speed boost!).
-Reclamation Pools: Changed bonus to +10% food from jobs (food usage reduction was equivalent to a tradition opener all on its own, not as logical a bonus (the flavor implies producing more food, not using less...)).
-Frenzy: Doubled both bonuses to +10% (to bring in line with e.g. Distinguished Admiralty).
-Cult of Personality: Removed war exhaustion reduction (this is a common modifier used in other government components).
-Cult of Personality: Buffed to provide +20% influence gain (was +10%).
-Workers' Councils: Rebalance of political power such that, assuming Decent Conditions living standards, Worker political power increased by 50% and Specialist political power increased by 12.5%. (This will start the two strata with 22.5 and 15.75 political power, respectively.)
-Fixed missing German localizations.

v1.4.5.3 (12-19-18)
-Planetmind Creativity: Now gives -10% pop housing and amenities use. (Had the same issues as Distributed Planning Systems.)

v1.4.5.2 (12-17-18)
-Direct Revelation wild cult MttH doubled (felt like they were stacking on top of each other too much), duration doubled (as they happen less frequently, they should last longer).

v1.4.5.1 (12-17-18)
-Fixed bug that prevented Warrior Hall upgrades in some cases.

v1.4.5 (12-15-18) Le Guin Improvements Phase 4
-Builder Caste: Changed to "Worker Caste," also gives 1 Menial Drone per 20 pops.
-Warrior caste: Instead of morale bonus, gives 1 warrior per 30 pops.
-Royal Caste: Instead of influence bonus, gives 1 Synapse Drone per 40 pops.
-Architect Expert Systems: Doubled bonus.
-Distributed Planning Systems: Now gives -10% pop housing and amenities use.
-Cosmic Choir now requires either pacifist or xenophile.
-New Cosmic Choir name list.
-Moved all base game government namelist definitions to one file (this will make it easier to override in any patch for the purpose).
-Crusader Kingdoms with FanSpi or FanMil are weighted heavily towards the Imperial Spiritualist and Imperial Militarist name lists (respectively).
-Crusader Orders no longer use regnal or dynastic names (not sure if this actually did anything in game, it was copypasta from CK).
-Changed 'lrsk_gov_var_gov_megachurch' token to 'lrsk_gov_var_gov_evangelical_franchise' to reflect the "new" name.
-Changed 'lrsk_syndicate' token to 'lrsk_syndicalist' because "syndicate" has a very different meaning in Stellaris.
-Changed 'lrsk_gov_var_gov_legionary_polis' token to 'lrsk_gov_var_gov_citizen_legion' to reflect the actual name of the government rather than its weird too edgy prototype.
-Clearing out a lot of obsolete cruft.

v1.4.4 (12-14-18)
-Workers' Councils: Buffed power bonus to woker +40%, spec +20%, halved happiness bonus (since it is now magnified further, and keeping them happy should be more of a challenge). Build speed bonus doubled to +10%.

v1.4.3.1 (12-12-18) - Hotfix: propagating localizations
-Yep.

v1.4.3 (12-12-18) - Le Guin Improvements Phase 3
-Direct Revelation: Removed modifier, effect is now based on random mostly beneficial events (wild cults and their added hedge preacher jobs).
-Added "Noble Republic" government, which requires Oligarch auth and Aristo Elite civic.
-Added "Crusader Order" government, which requires Oligarch auth, Spiritualist ethos, and both Aristo Elite and Chivalry civics.

v1.4.2.3 (12-10-18) - Still More Post-Le Guin Hotfixes
-Fixed bug where oligarchic form of Cosmic Choir had no start screen text.

v1.4.2.2 (12-10-18) - Post-Le Guin Hotfixes part 3.5
-Direct Revelation: Admin cap buffed to +20 to bring in line with "Divided Attention" (better things are coming for this civic, but in the meantime...)

v1.4.2.1 (12-10-18) - Post-Le Guin Hotfixes part 3
-Big Picture Thinker: now gives bonus to terraform and megastructure build speed.
-Reciprocal Planning Routines: Admin cap buffed to +20 to bring in line with "Divided Attention"

v1.4.2 (12-10-18) - Le Guin Improvements Phase 2
-Workers' Councils: Nerfed base bonus, incompatible with Shared Burdens, now increases happiness and political power of workers and specialists.
-Institutionalized Collectivism: Replaced "Not Dem" with "not Fan Auth"; removed ship, building, and district upkeep bonus. Now increases output of workers and specialists, and increases consumer goods output.
-Utilitarian Planning: Removed Dictatorship req, and no longer really a socialist-themed thing. Moved and nerfed upkeep bonus here, nerfed resettlement bonus.
-Proletarian Dictatorship: Removed Utilitarian Planning req, changed name to "Proletarian Regime."
-Automated World-Commune: Removed Utilitarian Planning or Public Works req.
-Populist Monarchy: Removed Philosopher King and Public Works req and no Authoritarian req, requires Institutionalized Collectivism.
-Social Bureaucracy: Removed Public Works req.
-Social Democracy: Removed Lifelong Learning and Public Works req, and not Authoritarian req (latter was redundant w/ democratic req), requires Institutionalized Collectivism.
-Communal Democracy, Socialist Plenary: Requires both Workers' Councils and Institutionalized Collectivism
-Pretender Hive: Has an Imperial variant with "Backup Overmind" heir.
-Return of Syndicalism as either "Syndicalist Congress" (Workers' Councils, Democratic authority) or "Syndicalist Conference" (Workers' Councils, Oligarchic authority)

v1.4.1 (12-09-18) - Le Guin Improvements Phase 1
-Changed Chivalry: Requires Militarist and Imperial or, with Aristocratic Elite, Oligarchic. Improves military leader skill levels, allows building Warrior Hall buildings which produce Knight jobs.

v1.3.3 (12-09-18) - Post-Le Guin Hotfixes part 2
-Removed an unneeded code line.

v1.3.2 (12-08-18) - Post-Le Guin Hotfixes
-Error with "OR {" should be "OR = {" fixed in name lists.
-Commented out missing references until needed.
-More legacy listings removed.
-Elected Clergy: faction_influence_add changed to pop_factions_produces_add
-Republicanism: leader_cost changed to leaders_cost_mult
-Utilitarian Planning, Reclamation Pools: pop_food_req_mult changed to planet_pops_organics_food_upkeep_mult
-Cult of Personality: country_resource_influence_mult changed to country_influence_produces_mult, changed slave happiness modifier to war exhaustion modifier (old modifier removed).
-Supremacist Demagoguery, Boundless Spite: Changed rivalry influence gain to increased max rivalries (old modifier removed).
-Enlightened Liberalism, Void Affinity, Astro-Prospecting Mainframe: Changed station build cost reduction to station outpost boost (old modifier removed).
-Business Lobby, Hoarder, Self-Aware Production Targets: country_resource_X_mult changed to country_X_produces_mult
-Lifelong Learning: Changed scientist cost reduction to scientist level bonus (old modifier removed).
-Institutionalized Collectivism, Eusocial Rhythm, Recursive Efficiency Analysis: ship_upkeep_mult changed to ships_upkeep_mult and planet_building_upkeep_mult to planet_structures_upkeep_mult
-Direct Revelations, Big Picture Thinker, Reciprocal Planning Routines: Changed to add admin cap (old modifier removed).
-Royal Absolutism : Changed to slower pop ethics shift speed (old modifier removed, this is a stopgap until I get something better).
-Public Works, Geosurvey Heuristics: planet_clear_blocker_cost_mult changed to deposit_blockers_cost_mult
-Automated Indolence: pop_robot_production_output changed to planet_jobs_robotic_produces_mult, unrest reduction changed to stability increase
-Planetmind Creativity, Distributed Planning Systems: edict_cost changed to edicts_cost_mult
-Royal Caste: Changed governor cost reduction to additional governor level (old modifier removed), country_resource_influence_mult changed to country_influence_produces_mult
-Gestalt Extroversion: diplomacy_influence_cost changed to diplomacy_upkeep_mult, changed the now-defunct "Federal Unity" bonuses to trust growth and cap.
-Reflective Polymorphism: Changed to flat -33% leader cost (old modifier removed).

v1.3.1 (12-07-18) - Stellaris 2.2 Le Guin Future-Proofing
-Updated compatible version number.
-Commented out or pruned various legacy entries.
-Crusader Kingdom government type has more specific requirements (civics in addition to ethos).
-Supremacist Demagoguery no longer bound to any authority type, but conflicts with Fanatic Purifiers (it was always supposed to be a lesser/poser version of that civic anyway.)
-New government types added for change to Supremacist Demagoguery.
-Changed Syndicalism government to Market Socialism. (But don't worry, the Space Wobblies will return in a new form someday!)
-Basic civics not available to Corporate authority.
-Updated Galactic Cartel, PMC, Evangelical Franchise, and Occult Cartel governments to be available to Corporate authority and civics. (Other custom megacorps will have to wait for new civics...)

v1.3 (11-25-18) - Better Names Project
-Complete rework of random name system to provide more flavor and distinction to empire names. Ranomly spawned empires should now have names that give you some indication of what their government is like (authority and/or ethos). Base game random names still exist and may show up, but are heavily out-weighted.
-Added new Purifier government types: Doom Horde (w/ Warrior Culture), Death Cult (w/ Exalted Priesthood or Elected Clergy), Citizen Legion (w/ Citizen Service).
-Fixed misc. typos.
-Libertarian Freehold ruler title is now "Chief Arbitrator."
-Republican Directory now requires Egalitarian ethos.
-Insurrectionary Lineage requirements greatly simplified, now requires Cult of Personality and Institutionalized Collectivism, some degree of Militarist ethos, and Imperial authority.

v1.2.4 (08-24-18)
-Hotfix for civic random pick weighting, civics added by this mod became 80% less likely to spawn due to a change in base game weights (maybe). Should now spawn on roughly par with base game civics.

v1.2.3 (06-12-18)
-Minor "Enlightened Liberalism" description change.
-Removed all "anomaly fail chance" related modifiers.

v1.2.2.1 (03-20-18)
-Fixed bug in "Cosmic Choir" government.

v1.2.2 (03-05-18)
-Removing deprecated/legacy cruft where possible.
-"Direct Revelation" changed to just require some degree of Egalitarian and Spiritualist because the previous requirements did not work as intended because you can't nest "OR" blocks in a civic prereq definition.
-Removing pleas for help with icon art.

v1.2.1 (03-04-18)
-New icons thanks to Meltup.

v1.2 (02-26-18) - The Gestalt Project
-Added gestalt civics (for Hive Minds and Machine Intelligences).
-Changed "Elected Clergy" to now boost to edict length and increase max faction influence.
-Buffed "Aesetic Virtues" because the growth bonus seems uncommonly small.
-Changed "Republicanism" to make recruitment cheaper rather than increase experience gain.
-Buffed "Utilitarian Planning" to double resettlement cost savings.
-Removed "Grandiosity" as it no longer makes sense with the new starport system.
-Added "Siege Mentality" civic (uses old "Grandiosity" icon) that increases starport defense effectiveness.
-Added "Cult of Personality" civic (makes up for SSR, below).
-Changed "Workers' Councils" to include improvement for starbase building build speed.
-Changed "Lifelong Learning" to reduce scientist recruit cost, increase governor skill levels, and increase leader experience gain.
-Changed "Institutionalized Collectivism" to reduce building and ship upkeep (slave unrest bonus didn't make sense on civic that did not require slavery allowed).
-Nerfed "Direct Revelation" effect to bring it in line with the "Courier Network" tradition.
-Removed "State Secular Rationalism" because its most interesting modifier was removed from the game.
-Removed legacy/dummy civics (new patch broke old saves, no longer needed).
-Government "Insurrectionary Lineage" now possible with "Institutionalized Collectivism" or "Cult of Personality".
-Some modifiers had to be changed to bring into line with 2.0 changes/removals.

v1.1 (11-24-17)
-Modified some descriptive flavor text, fixed typos.
-Changed PMC reqs: only Corporate Dominion + Citizen Service, no other civics.

09-22-17
-Fixed issue w/ new hive mind type ethos as civic restriction.
-Updated to using "has_valid_civic"
-Changed "Feudal Empire" to "Noble Empire" as alternative to new vanilla "Feudal Empire"
-Changed "Megachurch" to "Evangelical Franchise" as alternative to new vanilla "Megachurch"
-Changed "Occult Franchise" to "Occult Cartel"
-Changed "Elected Clergy" to somewhat increase edict duration and reduce edict cost, as duration is now modified by a base civic.
-Civic "Imperial Economy" now gets extra naval capacity rather than research sharing.

09-21-17
-Quick 1.8 update.
-Undid an error

08-10-17
-Fixed localization issue with PMC and RMF name randomization, other minor errors.

06-04-17
-Fixed localization issue with Quasi-Collective Consciousness AI personality.

05-25-17
-Fixed bug where "Communal Democracy" needed a legacy version of a civic.

05-23-17
-Tightened some government requirements to emphasize their role as "ideal forms."
-Added governments: "Private Military Contractor" and "Rationalist-Managerial Firm"

05-22-17
-Fixed missing start screen text for "Anarcho-Capitalism" government.

05-18-17
-Added "Megachurch" and "Occult Franchise" government types by popular demand.
-Added localization for above.
-Fixed localization typo.

05-13-17
-Reverted requirements for "Elected Clergy" and "Workers' Councils".
-Fixed a misc bug with government type selection.

05-12-17
-Fixed "Ascetic Virtues" to improve growth rate per new 1.6 modifier.

05-11-17
-Updated to 1.6.*
-Added "Automated Indolence" and "State Secular Rationalism" civics
-Civics "Elected Clergy" and "Workers' Councils" now require Democratic authority *or* Egalitarian ethics.

04-09-17
-Added "Robber Barons" and "Republicanism" civics
-Reworked a government type requirements.
-Added new government.
-Changed habitability bonus for Public Works from +10% to +5%
-Robber Barons bonus reduced to 5%

04-10-17
-Fixed (hopefully) issue causing nameless empires, lack of random name generation.
-Reworked some government requirements.
-Added a whole bunch of new governments.

04-11-2017
-Renamed "Captains of Industry" to "Enlightened Liberalism" and removed the Pacifist req.
-Made "Direct Revelation" require Pacifist or Egalitarian plus Spiritualist.
-Renamed "Robber Barons" to "Business Lobby".
-Renamed some government types.
-Reworked some government requirements.
-Added yet more governments!
-Changed "Enlightened Liberalism" to require not being Fanatic Authoritarian (some Enlightenment theories of rights and liberties are compatible with a degree of hierarchy and political inequality, but there has to be a limit).
-Changed "Enlightened Liberalism" to give 20% cost reduction on research and mining stations (research boost redundant with Materialist bonus).

04-13-17
-Bugfix: "Institutionalized Collectivism" now available if Fanatic Materialist (typo prevented this previously)
-Updated to 1.5.1
-Yet more new governments.
-Changed a number of civics requiring a particular ethos to simply require they *not* be the opposite. The general goal is to make civics a bit more open to use and allow for interesting mixes of apparent opposites.
-Loosened certain government type requirements.

04-14-17
-Buffed "Republicanism" and "Direct Revelation" (going forward I may mix up the bonuses provided by the civics a mit more)
-Added localization for non-English languages. (But it is all actually English, sorry! At least it's real text and not variables?)

04-15-17
-Fixed glitch in localization.
-Reworked some civic/gov requirements.
-New personality type and diplomacy for new government type.

04-17-17
-New unique icons!
-Fixed major bug in "Workers Council" (ship speed bonus not properly set)
-Fixed localization typo.
-Changed "Enlightened Liberalism" to require not being spiritualist rather than being materialist.
-Changed "Institutionalized Collectivism" to require not being democratic rather than dictatorial or imperial, removed requirement to not be egalitarian.
-Changed "Business Lobby" to give +5% to empire (rather than tile) minerals and energy output.
-Buffed "Lifelong Learning" (effects up to 15% from 10%)
-Buffed "Royal Absolutism" (bonus up to +25% from +15%)
-Buffed "Imperial Economy" (tech share up to +15% from +10%)
-Various government requirement tweaks.

04-21-17
-Removed "Pacifist" requirement for Worker's Councils.
-Updated localizations.


WARNING: I haven't exactly tested any of these in new games. So please do tell me if anything is broken, or unbalanced, or you have a better idea for something. It's very WIP right now.

http://steamcommunity.com/sharedfiles/filedetails/?id=901988941
