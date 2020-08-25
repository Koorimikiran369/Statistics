### Probability

- `Probability is the likelihood of an event occurring. Many events can’t be predicted with total certainty. The best we can say is how likely they are to happen,using the idea of probability.`

#### Event:
- An event is a set of outcomes(one or more) from an experiment. 
It can be like “Getting a Tail when tossing a coin is an event”, 
“Choosing a King from a deck of cards (any of the 4 Kings) is also an event”, 
“Rolling a 5 is an event” etc.

#### Events can be:

**Independent Event:**
Each event is not affected by other events.
  
    Example: Tossing a coin two times. The outcome of tossing the coin for the first time will not affect the outcome of the second event.

**Dependent (also called Conditional) Event:**
 An event is affected by other events. 
 
    Example: Drawing 2 Cards from a Deck. After taking one card from the deck there are fewer cards available, so the probabilities change!

**Mutually Exclusive Event**                    
Two events can’t happen at the same time. 

        Example: We can play football & rugby at the same time in the same football ground.
        
### Joint Probability:
- `Joint probability is the likelihood of more than one event occurring at the same time P(A and B). The probability of event A and event B occurring together. It is the probability of the intersection of two or more events written as p(A ∩ B).`

      Example: The probability that a card is a four and red =p(four and red) = 2/52=1/26. (There are two red fours in a deck of 52, the 4 of hearts and the 4 of diamonds).

**Conditions for Joint Probability:**

- One is that events X and Y must happen at the same time. Example: Throwing two dice simultaneously.
- The other is that events X and Y must be independent of each other. That means the outcome of event X does not influence the outcome of event Y.

    Example: Rolling two Dice.
    If the following conditions met, then P(A∩B) = P(A) * P(B).
    
**What will happen if we find the joint probability of two dependent events?**

   Let Event X is the probability there are clouds in the sky and Event Y is the probability that it rains. Everyone knows that rain comes from clouds. So rain can only fall when there are clouds in the sky. That means the presence of clouds will influence the chances of rain, and that means these two events are NOT independent!
Joint probability cannot be used to determine how much the occurrence of one event influences the occurrence of another event. Therefore the joint probability of X and Y (two dependent events) will be P(Y).
The joint probability of two disjoint events will be 0 because both the events cannot happen together.

So, unless or until we find how much the occurrence of one event influences the occurrence of another event, We cannot properly find the joint probability of two events. In order to solve this, Conditional Probability came to rescue us.

### Conditional Probability:
- `The conditional probability of an event B is the probability that the event will occur given the knowledge that an event A has already occurred. It is denoted by P(B|A).
So now, The joint probability of two dependent events becomes ‌P(A and B) = P(A)P(B|A)`

### Bayes Theorem:

We know that,
P(A and B) = P(A)P(B|A) and P(B and A) = P(B)P(A|B)
When we equate this we will get, P(A)P(B|A) = P(B)P(A|B), then

                    P(A|B) = P(A) P(B|A) / P(B)

**This is the Bayes theorem**

It tells: how often A happens given that B happens, written P(A|B),
When we know: how often B happens given that A happens, written P(B|A)
and how likely A is on its own, written P(A)
and how likely B is on its own, written P(B)

- In Machine Learning terms, Change A as Hypothesis and B as Evidence, then
*P(A|B) = P(A) P(B|A) / P(B)* becomes **P(H|E) = P(H) P(E|H) / P(E)**

This relates the probability of the hypothesis before getting the evidence *P(H) — prior probability, to the probability of the hypothesis after getting the evidence P(H|E) — posterior probability.* The factor that relates the two, **P(E|H) / P(E), is called the likelihood ratio.**

- ***`Bayes Theorem states that “The posterior probability equals the prior probability times the likelihood ratio”.`***

### Prior & Posterior Probability:

- Posterior probability is the probability an event will happen after all evidence has been taken into account.

- Prior probability is the probability an event will happen before you take any new evidence into account.

You can think of posterior probability as an adjustment on the prior probability

  **Posterior = ( Likelihood * Prior ) / Evidence**

### Hypothesis, Evidence & Likelihood:

- The hypothesis is your “guess” at what will occur. It is a testable assertion.

- Evidence will support or oppose the hypothesis.

- The Likelihood is the chance or probability that one thing will happen.
