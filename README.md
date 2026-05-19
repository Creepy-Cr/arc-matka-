# Arc Matka

Arc Matka is a wallet-based card result game built around scheduled sessions, clear bet types and published card result rules


## Repository Scope

This public repository contains product documentation, public release materials and user-facing references for Arc Matka

The implementation source is maintained in a private repository. This public repository is limited to documentation, product information, public release materials and user-facing references.

## What This Repository Contains

- Product overview
- Gameplay guide
- Session guide
- Card result rules
- Bet type explanations
- User-facing fairness notes
- FAQ
- Roadmap notes
- Public release policy files

## What Is Intentionally Not Included

- Application source code
- Smart contract implementation code
- Wallet sign-in code
- Server routes and services
- Privileged operation logic
- Environment files
- Secret signing material
- Build output or generated folders
- Private deployment settings

## Why Source Is Private

Arc Matka includes sensitive production logic, wallet session handling, privileged controls and contract-related work that should not be published in this public materials repository. Keeping implementation source private helps protect users, maintainers and the product while public documentation remains available for review

## Platform Overview

Arc Matka uses scheduled card result sessions. Users connect a wallet, sign in, choose a session, place a bet and track status through their wallet. Results are shown after reveal and eligible rewards can be claimed when available

## User Flow

1. Connect wallet
2. Sign in with wallet
3. Choose a session
4. Review timing and bet details
5. Place a bet through wallet confirmation
6. Wait for the result
7. Check My Bets
8. Claim rewards if eligible

## Session Types

Arc Matka uses three session types:

- Open Session
- Close Session
- Midnight Session

Each session has its own schedule. Times are shown in the user browser timezone where supported by the product interface

## Bet Types

Arc Matka supports:

- Single Number
- Jodi
- Unique 3 Cards
- Pair
- Three of Kind

See [docs/bet-types.md](docs/bet-types.md) for user-facing details

## Card Result Calculation

Three cards are revealed. Each card is converted to a digit value:

- Ace = 1
- 2 to 9 = same value
- 10, J, Q and K = 0

The three values are added. The last digit of the total is the final result number

Example: `2 + 5 + 7 = 14`, result `4`

Example: `A + 9 + K = 10`, result `0`

## Fairness Overview

Arc Matka is built around fixed schedules, locked betting windows and published result rules. Betting closes before reveal. Confirmed bets stay linked to the wallet that placed them. Results follow the published card calculation rules

This repository does not claim that live randomness is fully verified unless that status is confirmed in the product release materials

## Current Status

This public package is prepared for team sharing, public documentation review and product reference. It does not include implementation source

## Roadmap Summary

- Public docs
- Mobile polish
- Profile improvements
- Result history improvements
- Verified randomness integration when official provider details are available
- UX improvements

See [docs/roadmap.md](docs/roadmap.md)

## Documentation

- [Overview](docs/overview.md)
- [Gameplay](docs/gameplay.md)
- [Sessions](docs/sessions.md)
- [Card Results](docs/card-results.md)
- [Bet Types](docs/bet-types.md)
- [Fairness](docs/fairness.md)
- [FAQ](docs/faq.md)
- [Roadmap](docs/roadmap.md)

## Disclaimer

Arc Matka is a luck-based game. Winnings are not guaranteed. Users are responsible for understanding and following local rules that apply to them. Users should only risk funds they can afford to lose. Nothing in this repository is financial advice

## License

Documentation and product materials in this repository are licensed under Creative Commons Attribution 4.0 International. See [LICENSE](LICENSE)
