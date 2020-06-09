

### Implementation
We implemented the termination protocol and the loggings to handle node crash failures, link failures, and network partitions.

* `algo/nodes.py` contains the code for the participant and coordinator logic for 2PC, including part of the logging and the termination protocol logic.
* `algo/messages.py` implements messages, including `VoteReq`, `Vote`, `DecisionReq`, `Commit` and `Abort`.
* `algo/tasks.py` implements nodes' tasks such as node crashes and recovery.
* `tests` contains our unittest code. There are 8 testing scenarios, 5 of which test for node crash failures, 1 tests for link failures, and 1 test for network partition.

### Run Tests
To run the tests, run `python -m tests -v`.
