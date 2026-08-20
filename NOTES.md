# My notes from Bootcamp 2

I forked the repo and tried to understand how the self-resolving prediction market works.

### What I understood
- The market doesn't need anyone to press "Resolve".
- When the time comes, the Ritual Scheduler automatically calls the contract.
- The contract uses HTTP precompile to get data from an oracle and jq precompile to extract the number.
- If the oracle fails 3 times, the market becomes Invalid and everyone can get refund.

### What is still a bit confusing
- How exactly the retries are scheduled (the 200 blocks part).
- How the TEE executor is chosen each time.

I ran the local setup and tests to make sure everything works on my side.
Still learning, but the idea of autonomous contracts is really interesting.
