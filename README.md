# Bitcoin Sydney Socratic

This is an organizational repository to keep track of the Bitcoin Sydney Socratic agenda.

Meetings are held on Zoom (usually) on the first Tuesday of every month.
- Join our telegram chat: https://t.me/joinchat/F6jOnBpjJFXsGk3O5QRiyA
- Join our meetup (optional): https://www.meetup.com/Bitcoin_Sydney/events/278375421/
- Watch this repo to be notified of activity.

The meeting links are usually posted in the telegram chat just before it starts.

If you'd like to discuss a topic at the next meeting please make a pull request (log in to GitHub and click edit button at the top right of this page) or open an issue.

You can find IRC logs of a selection of previous meetings here: https://diyhpl.us/wiki/transcripts/sydney-bitcoin-meetup/

Videos of some of our meetings are on [Rumble](https://rumble.com/c/c-1038361).

## Meetings



### 2021-10

**Tuesday October 10th 7pm AEDT (8am UTC)**

_Discuss in [the issue](https://github.com/bitcoin-sydney/socratic/issues/2)_

### 2021-09

**Tuesday September 7th 7pm AEST (9am UTC)**

Lukas Aumayr will be taking us through his latest research [*Donner: UTXO-Based Virtual Channels Across Multiple Hops*](https://eprint.iacr.org/2021/855.pdf).
This applies the trick used in [*Blitz: Secure Multi-Hop Payments Without Two-Phase Commits∗](https://eprint.iacr.org/2021/176.pdf) (which he previously presented to us) to acheive _virtual channels_ with nice properties.
Virtual channels enable two parties without a direct channel to temporarily create a direct channel.
Although payments work fine without direct channels other layer-2 applications are not easily to do without direct channels.


This meeting will be recorded and put on rumble.

### 2021-08

**HOME GROWN EDITION**

**Tuesday August 10th 7pm AEST (9am UTC)** [Meetup Link](https://www.meetup.com/Bitcoin_Sydney/events/279898203)

Both presentations this week come from Bitcoin Sydney regulars!

#### Bitcoin <-> Monero Atomic swap

The [CoBloX](https://coblox.tech/) Sydney Research Lab is going to give us a technical run down on their Monero to Bitcoin atomic swap protocol.
Their atomic swap design is based on the [Succinct Atomic Swap](https://gist.github.com/RubenSomsen/8853a66a64825716f51b409be528355f) which was developed by Ruben Somsen.
There are several difficulties with BTC<->Monero atomic swaps since they use different elliptic curves and very different signature/transaction authorization schemes.

   - Code and further description https://github.com/comit-network/xmr-btc-swap
   - Paper: https://arxiv.org/pdf/2101.12332.pdf

I hope to tag on a discussion of the relevance of atomic swaps in a Bitcoin only future.

#### Differentially Private Payment Channels in Lightning

[Gijs van Dam](https://www.gijsvandam.nl) will do a walkthrough of his latest work on [differentially private payment channels](https://asciinema.org/a/6U2Y6iGrdwwvRoNqUYuOi9snP). 

### 2021-07

**Tuesday July 6th 7pm AEST (9am UTC) [Meetup Link](https://www.meetup.com/Bitcoin_Sydney/events/279162160/)**

This meeting will be more-or-less dedicated to discussion of fee bumping and layer-2 protocols.

#### Discussion on Layer-2 protocols and their Layer-1 requirements

   @ariard has been leading IRC meetings on this topic to try and get consensus around how to move forward. He'll joining us to lead the discussion. Topics to discuss:
   - Why do [BIP125] rules cause pinning attacks? What can be done about it?
   - Can we remove the absolute fee requirement from [BIP125]?
   - sponsorship idea by Jeremy Rubin: https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2020-September/018168.html
   - SIGHASH_IOMAP idea by @ariard: https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2021-May/019031.html
   - Does a layer 2 fee bumping and relay network make sense?
   - Package relay -- what is it and how does it help?
   - Time for full RBF?
   - Tentative Conclusions from the irc meetings.

Links:
   - Bitcoin problem page: https://bitcoin-problems.github.io/problems/fee-bumping.html
   - Summary of first irc meetings courtesy of Michael Folkson: [1](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2021-June/019079.html), [2](https://lists.linuxfoundation.org/pipermail/lightning-dev/2021-June/003077.html)

[BIP125]: https://github.com/bitcoin/bips/blob/master/bip-0125.mediawiki
