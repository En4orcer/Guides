> Information to include in the wp

***

### $CXCHE fungibility
Fungibility is the property of a good or a commodity whose individual units are essentially
interchangeable.
Bitcoins are not fully fungible.
Any two bitcoins have the same exact value.
But because all transactions are publicly available, it is common for bitcoin exchanges
to discriminate between bitcoins based on the owner or their history.
For example, some exchanges will attempt to block bitcoins, which have been confirmed as stolen or obtained illegally.
This becomes an issue because when not every exchange accepts the so called “dirty” bitcoins, the “dirty” bitcoins become less valuable.
The fungibility and privacy problem is solved in **$CXCHE** by CryptoNote protocol.
Transactions in **$CXCHE** are untraceable and unlinkable.
**$CXCHE** provides anonymity and privacy using cryptographic technology of ring signatures.
All transactions signed on behalf of a group so that it is impossible to determine who exactly from the group signed the transaction and, accordingly, one can not say with certainty who carried out the payment.
The more participants in the group, the more confidential the operation is.
In addition, the transactions cannot be associated, – even if outgoing transactions are untraceable, everyone may still be able to see the transactions you have received.
However, by using a variation of the Diffie-Hellman exchange protocol, a receiver has multiple unique one-time
addresses derived from his single public key. 
After funds are sent to these addresses they can only be redeemed by the receiver and it would be impossible to cross-link these transactions. 
Unique one-time addresses and ring signatures of transactions are providing resistance to blockchain analysis. 
Every transaction only increases entropy and creates additional obstacles for those who wish to dig into financial operations with **$CXCHE**.
Resistance to the analysis, in turn, provides a very important characteristic inherent in real **$CXCHE** money, – fungibility.
Fungibility of money means that all units of one denomination have the same purchasing power.

### Difficulty Algorithm

*“The problem of hash rate instability has been well known for many years in the altcoin
community. Multipool mining, where miners could quickly switch between mining coins with
compatible Proof of Work algorithms, led to hash rate oscillation and instability. This rapidly
switching hash power would often lead to unpredictable confirmation times, and long periods
with very slow blocks. There were also more serious problems when coins had widely
divergent market values, which could leave the smaller coin vulnerable to miners gaming of
the difficulty algorithm, and manipulating timestamps”* - https://medium.com/@Mengerian/bringing-stability-to-bitcoin-cash-difficulty-adjustments-eae8def0efa4

In 2016 Karbo mitigated to some extent this problem by changing the default CryptoNote
difficulty algorithm to the one proposed by Scott Roberts called “Zawy difficulty algorithm”.
The author of the difficulty algorithm developed a better version of his algorithm and it is proposed to update difficulty
algorithm to one of his newest versions: “LWMA (WHM)” or “The Simple DA” for
better protection against hashrate attacks. The LWMA (WHM) algorithm was implemented
after the attack in which vulnerabilities of previous version were exploited.
To mitigate part of other mentioned threats one solution that is considered is to change the
POW algorithm.
One of the possible solutions against hashrate attacks, which are mostly conducted by
renting hashing power on the Nicehash and similar services, is to change POW hashing
algorithm to make it incompatible with Nicehash and thus remove from multipool hoppers the
possibility to switch to $CXCHE when it’s profitable for them.
The second reason is the threat of ASICs, developed for the CryptoNight algorithm. ASICs
will cause undesired centralisation of mining and hashing power. From the other hands,
ASICs provide large hashrate that is the best protection against attacks on POW based
coins that $CXCHE was suffering. Therefore we consider to stay ASICs-compatible given the
fact of presence of at least four vendors offering ASICs on the market.

### Blockchain monetary deposits with interest rates
You can safely deposit your Cache with some interest rate.
In general it allows users to “lock” some of their $CXCHE for a while (from 1 month to a 1 year)
and after some time, withdraw it back with some interest as a part of main Cache supply.
Longer period gives users a bigger interest rate.
Deposits are implemented via new types of transaction output/outputs. It includes amount,
destination key (or keys) and time (expressed in blocks) to lock. Transaction itself contains the
field unlock time but output-specific parameters is much convenient, because user may want to
sent some money back as change (and surely doesn’t want them to be locked). The transaction
is included in the blockchain as usual and the counter starts.
When the lock expires user can spend this output as usual, but the new transaction volume
will be increased with the interest.
For example, if user makes a deposit of 1000 $CXCHE for 1 month an annual interest rate will be about 0.41%.
This is broken up in to 5 tiers: <5k, 5-10k, 10-15k, 15-20k, >20k.
It also means that deposits act as new source
of emission.
Cache multi-signature core feature enables a common ownership for any $CXCHE units
and deposits in particular. A family can store their $CXCHE savings in N-of-N deposits, which
means that only all members together can withdraw the money. Company can keep its capital
in M-of-N address, which is redeemable only by at least M members out of N.
Interest rate depends deposit time and varies from 1 month to 1 year. The latter case
is the most profitable (gives user maximum possible profit — 8% of their deposit).

### Crypto assets intrinsic value
*“Everyone can create money, the problem is to get it accepted”*

Hyman Minsky, an American economist
The target of stable coin design requires that this crypto asset has certain intrinsic value.
Without this value it is possible to build stable coin only with exogenous factors involved. In
other words manually managing its value by market interventions. There is no the only
opinion regarding whether crypto assets have its own intrinsic value or not. Some authors
claim that crypto assets do not have any intrinsic value. Some authors on the other hand
speak about this value represented by mining infrastructure.
Proof of Work (PoW) algorithm is usually criticised for excessive waste of energy on the one
hand and it is postulated that crypto assets based on PoW consensus do not have intrinsic
value on the other. “The criticism stems from the belief that Bitcoin violates Mise’s
regression theorem of money because it is not backed by a commodity.” However mining
infrastructure consuming megawatts of electricity is actually a commodity and if we accept
the fact that it represents intrinsic value of particular crypto asset than we admit that mining
infrastructure actually represents this commodity backing and energy spent on mining
represents the real value of such an asset. The more real world resources we attract for
mining the higher is crypto asset capitalisation. One can say that cryptocurrency is backed
by the energy spent on its mining.

*“Bitcoin production seems to resemble a competitive market, so in theory miners will produce
until their marginal costs equal their marginal product. Break-even points are modeled for
market price, energy cost, efficiency and difficulty to produce. The cost of production price
may represent a theoretical value around which market prices tend to gravitate.
It seems to be the case that the marginal cost of bitcoin production matters in value
formation. Instead of approaching bitcoin as a digital money or currency, it is perhaps more
appropriate to consider it a virtual commodity with a competitive market of producers.”*

Any mineable crypto asset has a so-called positive feedback loop, which means that when
the price of crypto asset decreases or block reward is decreasing, “mining” becomes less
profitable and some “miners” will be forced out of business. When there are less miners, the
network automatically adjusts to decrease the difficulty of the cryptographic problems and
therefore makes “mining” profitable again. In other words, proof of work mineable crypto
asset is designed to make “mining” barely profitable on average.
The main idea of those who believe in crypto asset intrinsic value is based on the fact that
production or mining being a competitive process represents the value which we are looking
for. In that sense we can call $CXCHE and any other mineable crypto asset a commodity
money backed by electricity and hardware expenditure consumed for network support. This
approach will let us to find endogenous factors or data from blockchain to first estimate and
than keep crypto asset value stable over time without relying on any third party or
exogenous impact. This is the key point in building such a system because any third party
involved in a process could be compromised and/or hacked over time.
Previous works like Ferdinando M. Ametrano’s proposal relied on some exogenous
commodity indexes consisting from crude oil and wheat, but we think that it makes sense to
peg crypto asset to electric energy as a commodity stable in its value. Difficulty represents
this energy spent on mining and therefore, from our point of view, difficulty is endogenous
factor which in the best way reflects crypto asset intrinsic value. Difficulty gives us real
estimate of mining efforts expressed in electric energy and hardware commodity costs spent
in real world on our crypto asset network support and emission.
Scott Roberts in his blog proposes a solution how to use blockchain data to determine the
coin price being outside, real world parameter: “Difficulty is exactly proportional to network
hashrate, and network hashrate is closely proportional to coin price”. Our solution is
based on his work, that finds confirmation by the research of Vitalik Buterin, published in his
blog post, where he describes methods of the decentralized measurement problem.
According to Buterin, there are two known major classes of solutions: exogenous solutions,
mechanisms which try to measure the price with respect to some precise index from the
outside, and endogenous solutions, mechanisms which try to use internal variables of the
network to measure price. We chose second method which was independently
discovered and described by Scott Roberts.

The research of Vitalik Buterin confirms Scott Roberts’ idea: to measure the price of a
currency endogenously, what we essentially need is to find some service inside the network
that is known to have a roughly stable real-value price, and measure the price of that service
inside the network as measured in the network’s own token. Examples of such services
include:
- Computation (measured via mining difficulty)
- Transaction fees
- Data storage
- Bandwidth provision

A slightly different, but related, strategy, is to measure some statistic that correlates indirectly
with price, usually a metric of the level of usage; one example of this is transaction volume.
Statistical methods, however are prone to be manipulated therefore we will not use them.
Aside manipulations, “...the problem with all of these metrics is, however, that none of them
are very robust against rapid changes due to technological innovation” he adds.
Therefore we have to include Moore’s Law compensation. As Buterin states, “difficulty is a
function of both price and Moore’s law, and so it gives results that depart from any accurate
measure of the price exponentially over time.” “The first immediate strategy to fix this
problem is to try to compensate for Moore’s law, using the difficulty but artificially reducing
the price by some constant per day to counteract the expected speed of technological
progress; we’ll call this the compensated naive estimator”.
Having determined the leading factor influencing crypto assets, we can proceed with an
attempt to estimate the crypto assets fair value, for which we take as a basis the suggestions
of Scott Roberts. The basis for his approach is the assumption of a relationship between
the crypto asset price and the mining cost, ideally energy costs. The equation is valid for the
PoW (Proof of Work) mining algorithm:
```
P1 * R1 / D1 * L1 = P2 * R2 / (D2 / M) * L2 (1)
```

where,
`1 and 2=` moments in time 1 (now) and 2 (future);
`P =` USD price per crypto asset unit;
`R =` reward, crypto assets units per block;
`D =` PoW mining difficulty;
`M =` Moore’s Law adjustment which represents the reflective change over time in the mining
equipment productivity (H/s), is calculated as 2^n, where n is the number of doubling
productivity periods;
`L =` loss factor, equal to the estimated volume of lost crypto assets units due to private keys
loss. Coefficient 1 means that 100% of crypto assets units are available, a coefficient of 0.75
means that every fourth unit of crypto assets is unavailable due to the private keys loss.
If hash power is not able to keep up with coin price (which is a temporary effect), the value
would be larger than expected. Otherwise, the real-world value slowly decreases as hashing
efficiency increases, which may be a desired effect if it is for dev fees because software gets
outdated. But Moore's Law has gotten very slow for computers. Hashing should get closer to
being a constant hardware cost per hash. Also, electricity is more than half the current cost
of hashing and could soon be 3/4 or more of the cost. Worldwide electricity cost is very
stable and possibly the best single-commodity measure of constant value.
The same equation can be rewritten simpler:
```
P1 * R1 / E1 * L1 = P2 * R2 / E2 * L2 (2)
```

where,
`E =` mining electricity consumption in kWh.
Now we rewrite the equation having in mind that P1 = P2 to define R2 (next reward for the
block):
`R2 = R1 * (D2 / M) / D1 * L1 / L2 (3)`
The logic that determines the next block reward is as follows:
`R1 =` previous block reward;
`(D2 / M) / D1 =` increase in complexity, that is, an increase in the mining capacity leads to an
increase in the crypto asset price, taking into account the Moore’s Law adjustment;
`L1 / L2 =` over time, an increasing number of crypto assets units are lost due to the private
keys loss, a reduction in the issuance of crypto assets in this way increases its price.
We have to mention that this equation gives crypto asset fair price estimate and does not
take into account the speculative component, the so-called pumps and dumps.
