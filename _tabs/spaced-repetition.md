---
title: Spaced repetition
icon: fas fa-hourglass-half
order: 3
---

Spaced repetition using flashcards is one of the most effective methods to memorize things.
If you want to learn more about it, you can start on [article on Wikipedia](https://en.wikipedia.org/wiki/Spaced_repetition){:target="_blank"} or check out
[this wonderful comic strip](https://ncase.me/remember/){:target="_blank"} from Nicky Case.

## Recall level

Every card detected in your notes has a so called "recall level" associated with it which indicates how well you remember it. It also represents the number of days after which it
will be queued for review again.

## Multipliers

When you are testing yourself, the recall level changes based on how well you remember the card. The theory is simple - if you remember it well
the recall level goes up, otherwise it goes down.

**Recall** uses a simple algorithm and multiplies the current recall level by a constant and there's a constant defined in your configuration
for each of the review results. By default, these constants are 2, 0.5 and 0, which in practice means that

- if you click Remembered, the recall level will be doubled;
- and if you click Struggled, the recall level will be halved;
- if you click Forgot, the recall level will go back to 1 (minimum value).

<!--
## Alternative setup

Some articles on spaced repetition recommend that if you forget a card, its recall level should go back to 1 and it should appear
in your review the next day. If you want to use this approach, it can easily be achieved with the following configuration:

| Setting used               | Value | Meaning                                     |
| -------------------------- | :---: | ------------------------------------------- |
| Multiplier for Rembembered | 2     | Recall value will be doubled                |
| Multiplier for Struggled   | 0.5   | Recall value will be halved                 |
| Multiplier for Forgot      | 0     | Recall value will be set to 1 (the minimum) |

Naturally, other values for the constants are also possible so you can fine tune your algorith as you see fit. The above is just one of the alternatives.
-->
