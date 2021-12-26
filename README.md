# MILKPATCHED
RJW's milkable colonists - Now with less absurd debuffs, more milk, overfilled breasts and quicker growth.


Notable changes (UPDATE 1.0):

LACT-X, LACT-MAX & HYPER LACT-MAX no longer fucking cripple your pawns.
I mean, hyper LACT-MAX still does the brain damage thing because I think it's neat and is actually balanced instead of just kneecapping your pawns for fun, but they no longer cap your pawns consciousness/manipulation just because their tits are leaking milk.
They still cause temporary trouble with manipulation and moving at first consumption, but it settles down once the high wears off.
Only hyper LACT-MAX still has some permanent debuff beyond the brain damage, but it's just -10% to mov & man, so you can counter it with go-juice, bionics, neural supercharge or whatever other shit you have to increase those numbers.

Milk output significantly increased. Like, it's almost 3x more milk than default.
You can almost feed a colony off it's own milk if they're all women, but then again this mod is 50% to jack off, so it's not like realism is a big deal.
Still, if you care enough to change it, it's just the RaceMilkPatch.xml, just look in there, find the milkamount (currently 36, originally 12) and change all 3 instances to the amount you want, restart rimworld and voila.
Don't particularly understand how a racepatch alters the output for regular humans too, but I'm not complaining.

Changed breast growth due to breasts being over max fullness.
Now you can grow breasts beyond huge without using Hyper LACT-MAX going over 100% fullness without milking a pawn will have her breasts grow 0.05 severity every 30k ticks (roughly ~30 seconds with on the 4x speed mod, or half an ingame day), up to 1.6 severity, which is somewhere in the colossal range (I think?) It might be too slow, maybe, but it's still wayyyyy faster than the original, and goes beyond the original max 0.9 severity.

Added a little "Overfilled" Health heddiff, to represent discomfort and pain common with accumulated milk in the breasts without lactation, as a quick little counterbalance for increasing your pawns breasts for free and also because it makes my dick hard.
The health hediff adds +5% pain and nothing else. It comes coupled with a thought hediff that's -2 mood. Once your pawn is milked, the health hediff goes away the next check (30k ticks, half a day).
The thought remains for a full day, but goes away if they've been milked after this time passes.

UPDATE 1.1:

My small brain has come with simple changes to the way I implemented the overfilled breasts mechanic. Simply put, I initally used an existing check to add the overfilled hediff.
This is cool and good, as the check already existed, performance wouldn't be affected at all. But I couldn't figure out how to remove the hediff and added another check to see if fullness went below 100% and if so, remove the hediff, if it existed.
Now, with the benefit of a couple more minutes of fucking around, I found out I can just make the hediff itself lose severity over time like much other hediffs in-game.
So now I don't need that extra if condition, probably causing a little less lag every check.
It goes down by 1.0 severity per day, and goes up by 1.0 per day without milking, ideally ending in +0.0 severity/day so it won't decay while a girl is still full.

"Overfilled" hediff now also increases sex drive by 10%, mostly because it makes my dick hard. You can easily edit it out of the .xml if you don't like it. Also can
change the severity fall rate per day too, if you think it needs adjusting.

Milk fullness can now go all the way to 200%, both because it's a cooler number and allows for you to store more lactation at once, and also because it makes my dick hard.

Decreased breast growth rate ( 0.05f(5%) -> 0.005f(0.5%) ); previous rate meant that barely a few days overfilled would get women to have colossal breasts which, while hot, felt a bit too absurd for me.
This should make it so breast severity jumps ~0.009 severity every 1/2 day, or ~0.020 every day.
This should make it so breast severity grows ~0.300 every quadrum, and up to ~1.2 a year, assuming they're never milked, which means even a girl with tiny breasts could become colossal in the span of a year, assuming permanent lactation and no milking whatsoever. Maybe this is still much? I feel it's adequate, whatever.

FAQ (I'm lying, no one ever asks these, I'm making them up):

-Anon, why did you make this mod?
Lactation makes my dick extremely hard, and seeing how they crippled it in the original mod made me and my dick sad :(

-What are your previous experiences on modding, rimworld or otherwise?
Literally none. I learned how to edit .xmls and decompile/recompile C++ exclusively here, which explains my incompetence partly.

-can you help me with [MODDING ISSUE HERE]?
Chances are probably not, given my aforementioned incompetence, but sure, just ask for the milk guy on /rwg/. I might be there for a while.

-can you change [THING] in this mod?
Can't you? Seriously speaking, yeah probably, but it's really simple stuff and I reckon you could change it if you spent an afternoon figuring out dnspy or another simple tool.
I'm being a dick. Ask me about it and I might do it, if it seems reasonable.
