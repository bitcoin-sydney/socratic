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


### **2022-06 June 28th 7pm AEST (9am UTC) -- RECORDED**

ORDINAL NUMBERS NFTs EDITION

Casey Rodarmor will present his "Satoshi Ordinals" colored coin proposal. This proposal gives every satoshi a unique positoin in the total set of satoshis whose identity doesn't change even after a transaction spends it.

The proposal: https://github.com/casey/ord

### 2022-04

**Tuesday April 26th 7pm AEST (9am UTC) -- RECORDED**

SILENT PAYMENTS EDITION

Sydney Socratic Regular Ruben Somsen will be presenting his latest breakthrough: Silent Payments.
This is a scheme for taking a static address and deriving a new one from it yourself before sending to it without interacting with the receiver and without anyone other than the receiver being able to link the two addresses.
Existing schemes like [BIP47](https://github.com/bitcoin/bips/blob/master/bip-0047.mediawiki) do this by signalling extra data through the blockchain.
Silent payments don't need this so they are more efficient and leave no trace that this protocol is even being used.
The main downside is that it is more computationally expensive for the receiver to find payments.

- Mailing list post: https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2022-March/020180.html
- pre-BIP: https://gist.github.com/RubenSomsen/c43b79517e7cb701ebf77eec6dbb46b8

### 2022-03

**Tuesday March 29th 7pm AEDT (8am UTC) -- RECORDED ([video](https://rumble.com/vz3i3u-frost-the-future-of-schnorr-multisignatures-on-bitcoin.html))**

Bitcoin Schnorr/Taproot Threshold Multi-signatures edition.

What will the multi-sig setups of the future look like?

This month we're going to be talking to Jesse Posner @jesseposner about the ongoing effort to implement Schnorr threshold multi-signatures. With these you can create a 2 of 3, or a 3 of 5 etc that is indistinguishable from a regular single key spend.
Background watching/reading:

1. The Quest for Practical Threshold Schnorr Signatures - Tim Ruffing - CES Summit '19: https://www.youtube.com/watch?v=Wy5jpgmmqAg

2. FROST: Flexible Round-Optimized Schnorr Threshold Signatures: https://eprint.iacr.org/2020/852.pdf

In progress implementations:

1. https://github.com/ElementsProject/secp256k1-zkp/pull/138#issuecomment-1007655837

2. https://github.com/LLFourn/secp256kfun/tree/frost



### 2022-01

**Tuesday December 25th 7pm AEDT (8am UTC) -- RECORDED**

**CFD DEGEN EDDITION**

The main even for this week's Socratic is Sydney based Bitcoin research lab [CoBloX] presenting their Bitcoin *Contract for a Difference* protcol being used by [ItchySats].
This is effectively a layer-2 DLC in a channel that can be *rolled over*.
Unlike a typical DLC on a price at a time X, the parties can continually move back the expiration time if they agree to do so.

- ItchySats announcement: https://itchysats.medium.com/itchysats-roadmap-to-the-most-awesome-bitcoin-dex-464a42bf4881
- CoBloX technical protocol explanation: https://comit.network/blog/2022/11/01/cfd-protocol-explained

If we have time after that we'll chill and discuss [`OP_CTV`] developments (and drama) or whatever else people want to bring up.
This bit won't be recorded.

### 2021-12

**Tuesday December 7th 7pm AEDT (8am UTC) -- RECORDED**

**ZERO BASE FEE EDITION**

This week Rene Pickhardt will present his research on lightning route opimtization "Optimally Reliable & Cheap Payment Flows on the Lightning Network".

1. The paper: https://arxiv.org/pdf/2107.05322.pdf
2. Mailing list post: https://lists.linuxfoundation.org/pipermail/lightning-dev/2021-August/003203.html
3. Earlier paper: https://arxiv.org/pdf/2103.08576.pdf

### 2021-11

**Tuesday November 2nd 7pm AEDT (8am UTC)** [meetup link](https://www.meetup.com/Bitcoin_Sydney/events/281708383/)

*dicuss in the [issue](https://github.com/bitcoin-sydney/socratic/issues/3)

This week we'll be discussing the following topics:

1. Package relay:
   1. Mailing list post: https://gist.github.com/glozow/dc4e9d5c5b14ade7cdfac40f43adb18a
   2. PRs: (i) https://github.com/bitcoin/bitcoin/pull/22290 (ii) https://github.com/bitcoin/bitcoin/pull/22674
2. PTLCs in Lightning with Taproot
   1. https://lists.linuxfoundation.org/pipermail/lightning-dev/2021-October/003278.html
3. BONUS: If there's time it'd be fun to talk about what would happen to the value of Bitcoin in a 51% attack:
   1. Writeup that started discussion: https://gist.github.com/fernandonm/ef9721bacf7284e039caf39ba2a07258
   2. thread 1: https://twitter.com/fnietom/status/1452335538573389828
   3. thread 2: https://twitter.com/SomsenRuben/status/1452365125852274695
   4. follow up: https://gist.github.com/fernandonm/6844b85973c3a3b7ceb92979c8a7281d


### 2021-10

**Tuesday October 5th 7pm AEDT (8am UTC)** [meetup link](https://www.meetup.com/Bitcoin_Sydney/events/281087671)

Lloyd Fournier will be presenting his "DLCs/betting over twitter" project [`gun`](https://github.com/LLFourn/gun).
See the documentation at https://gun.fun.
This bit will be recorded.

Then we'll have a non-recorded discussion on [TAPLEAF_UPDATE_VERIFY](https://lists.linuxfoundation.org/pipermail/bitcoin-dev/2021-September/019419.html)

### 2021-09

**Tuesday September 7th 7pm AEST (9am UTC)** [Meetup Link](https://www.meetup.com/Bitcoin_Sydney/events/280479952/)

Lukas Aumayr will be taking us through his latest research [*Donner: UTXO-Based Virtual Channels Across Multiple Hops*](https://eprint.iacr.org/2021/855.pdf).
This applies the trick used in [*Blitz: Secure Multi-Hop Payments Without Two-Phase Commits???](https://eprint.iacr.org/2021/176.pdf) (which he previously presented to us) to acheive _virtual channels_ with nice properties.
Virtual channels enable two parties without a direct channel to temporarily create a direct channel.
Although payments work fine without direct channels other layer-2 applications are not easily to do without direct channels.


This meeting will be recorded and put on rumble.

### 2021-08

**HOME GROWN EDITION**

**Tuesday August 10th 7pm AEST (9am UTC)** [Meetup Link](https://www.meetup.com/Bitcoin_Sydney/events/279898203)

Both presentations this week come from Bitcoin Sydney regulars!

#### Bitcoin <-> Monero Atomic swap

The [CoBloX] Sydney Research Lab is going to give us a technical run down on their Monero to Bitcoin atomic swap protocol.
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
[CoBloX]: https://coblox.tech/
[ItchySats]: https://www.itchysats.network/
[`OP_CTV`]: https://bitcoinops.org/en/topics/op_checktemplateverify/
