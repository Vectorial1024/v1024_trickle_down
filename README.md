# Trickle Down
[WIP] Player internal trades will now transfer credits if possible. Greatly inspired by Player-Faction Accountant.

(links etc)

> Financial management, that's how simple it is!

## Background Info
It is very well known that in vanilla, player-to-player trades never transferred any money. This can easily cause stations to run out of money when buying resources from NPC traders, especially when there is a partial production chain that is not yet fully self-sufficient.

The "obvious" solution to this is to let player-to-player trades transfer the money, just as Player-Faction Accountant did. Egooft allegedly also tried this in the 5.0 beta, but quickly removed this feature from the 5.0 release. As I have later discovered, it turns out, not having the money to pay for wares will disrupt logistics because the buyer will now issue very good but impossible ("cannot pay") buy offers. The AutoTrade script will be bricked by this by repeatedly selecting the same impossible offer.

At the end of the day, we just want to have a natural, hands-free way of making sure all the stations have enough money for their operations.

So, instead of a strict requirement (no money no trade), this mod chooses to be more lenient: trade first, and then pay if possible.
