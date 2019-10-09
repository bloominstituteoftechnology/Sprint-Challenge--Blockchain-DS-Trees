# Blockchain Sprint Challenge

Welcome to the ground floor!  Satoshi Brian is giving you the chance to be the first people to mine Lambda Coins.  However, you'll have to compete with your fellow students to cash in.  

Your task is to use your knowledge to write a mining program, similar to the ones you have been working with, to mine coins for the Lambda Blockchain.  

The Lambda blockchain server works the similar to the demos this week, _but it uses a DIFFERENT Proof of Work Algorithm._

Multi-Ouroboros of Work Algorithm
    - Find a number p' such that the last six digits of hash(p) are equal
    to the first six digits of hash(p')
    - IE:  last_hash: ...AE9123456, new hash 123456BA8...
    - p is the previous proof, and p' is the new proof

Some things to keep in mind:
* With everyone mining at once, it may take a long time to actually mine a coin on the main server. _You will lose the contest most of the time!_
* There is a test server that you can test your code on:  lambda-coin-test-1.   As before, you can change the server that the miner uses by including it in the command to run the miner:  `python3 miner.py https://lambda-coin-test-1.herokuapp.com/api`
** Please only mine against the test server to test your code - stop mining when the test is over
* The main server, and the competition, is the default and will run with `python3 miner.py`
* Please change your name in `my_id.txt` to something recognizable


Some Strategy Suggestions:
* Don't forget to install dependencies with `pipenv install` and run them inside `pipenv shell`
* _Think about what will happen if your strategy is the same as the example from class.  If you start at 0 and count upward, and someone else does the same thing, but they start earlier or have a faster computer, what will happen?_


API Endpoints:

`/api/mine`
POST - Submit your name and a proposed proof for validation.  If the action is unsuccessful, you will receive an error message.  If successful, it will return:

{
    'index': block.index,
    'transactions': str(block.transactions),
    'proof': block.proof,
    'previous_hash': block.previous_hash,
}

Failure:
{"message": "Proof valid but already submitted."}

-or-

{"message": "Invalid Proof"}


`/api/full_chain`
GET - Returns the full chain in JSON format


`/api/totals/`
GET - Returns the current total for each ID in the chain


`api/last_proof`
GET - Returns the last proof used to mine a block, and the current difficulty level.  Note that `difficulty` is currently set to a fixed number and can be ignored...for now!

{
    'proof': last_proof_value,
    'difficulty': ChainDifficulty.objects.all().last().difficulty
}
