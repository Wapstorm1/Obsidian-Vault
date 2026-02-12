- How you define risk
- When you would allow known bugs
- What makes a release a “no-go”
- How you separate user risk vs business risk
- Tell me about a mistake you made in QA.
- What kind of tester are you not?

- What do you struggle with as a QA?
  I feel most challenged when dealing with complex features that involve multiple systems or hidden dependencies. In those situations, I’ve learned that the key is asking more clarifying questions early and mapping out risks before jumping into testing. It’s an area where I’m actively improving — becoming more structured and confident in handling complexity.
-  How do you decide whether a bug is frontend or backend?
  I reproduce the issue, check the API response, and compare it with what the UI shows. If the backend response is correct but the UI is wrong, it’s frontend. If the response itself is wrong, it’s backend.
- About big amount 8allocate bug - why they did not catch it earlier?
  At that stage we were validating logic correctness but not testing with realistic transaction amounts. The system worked under small values, so the edge case with larger amounts wasn’t exposed. It wasn’t negligence — it was a coverage gap that became visible only under realistic conditions.
- What did you learn?
  I learned that validating edge conditions and real-world data scenarios early can prevent high-impact failures later, especially in financial systems.