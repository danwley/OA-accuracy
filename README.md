🎯 **Target Audience:** Chess platforms (like chess.com), streamers, commentators, and players interested in a richer game analysis.

# Outcome-Adjusted (OA) Accuracy in Chess

Welcome to the OA Accuracy repository! Here, we're exploring an alternative yet complementary metric to traditional chess accuracy, aiming to better represent real-game dynamics, especially in low time control formats.

Check out this motivation from GothamChess, one of the biggest chess streamers/coaches out there.

Figure comparing traditional accuracy to OA accuracy is all you need potentially. They are two ends of the extreme- evaluation according to the engine vs evaluation according to what actually happened in the game.

### 🛠 How It Works
After every move, a traditional engine computes the evaluation difference. If you don't lose eval from a move, you don't lose accuracy. If your move lost eval (e.g., a blunder), then your accuracy drops.

OA accuracy, on the other hand, takes into account your opponent's responses. If your opponent did not punish a blunder that you made, or an innacuracy, and so forth, you won't lose OA accuracy.

For example, you might play a gambit line in the opening. Your traditional accuracy usually suffers because the gambit is an inaccuracy. However, it's often the case that your opponent won't know the correct responses to your gambit/unusual opening line (this is often why players choose such moves). Thus, if your opponent doesn't capitalize on the gambit, it should arguably be considered the best move (depending on the opponent's response).

**The core principle:** If you make a move that loses game advantage (according to engine evaluation), but your opponent does not gain advantage, relative to the evaluation before your move, then the move's practical impact wasn't negative. Hence, it shouldn't heavily impact your OA accuracy.

**Example:** The position is equal with evaluation 0. You blunder and the advantage drops to minus 3. However, your opponent does not take advantage, and after their move, the evaluation bar rises to +2. Under traditional measures, your move would lose accuracy. With OA accuracy, you are not penalized for moves that result in equal or better positions.

**Include example from an actual game. Ask for the best move? Ask for the follow-up.**

Moments that Gotham alluded to something similar to OA accuracy: 16:00, 22:00

<a href="http://www.youtube.com/watch?feature=player_embedded&v=nTQUwghvy5Q" target="_blank">
 <img src="http://img.youtube.com/vi/9Ov93YjTZ70/mqdefault.jpg" alt="Watch the video" width="480" height="270" border="10" />
</a>

### Why OA Accuracy?
In the world of chess, a player's decision can be a blend of theory, intuition, psychological play, and time management. While traditional engine accuracy offers valuable insights, there's a space for understanding the effectiveness of moves in practical play. Enter: OA Accuracy.

<details>
<summary>📖 Background</summary>
Traditional accuracy reflects the theoretical best move.

OA accuracy respects real-life game dynamics, including the psychology of play and time pressures, especially prominent in formats like bullet or blitz.

### Why we can't replace traditional accuracy

- Might encourage bad practice from players. It has to be stated that OA accuracy reflects the other side of the extreme - while traditional accuracy uses the best moves according to an engine, OA accuracy targets 

##### Open Problems & Current Drawbacks of Traditional Accuracy

- **Not Reflective of Practical Play:** Traditional accuracy strictly follows engine recommendations, often overlooking real-world tactics and strategies that players employ, especially under time constraints.

- **Missed Psychological Tactics:** Players sometimes employ moves that prey on their opponent's psychology or anticipated responses. These moves might be considered inaccuracies by engines but can be game-winners in practice.

- **Bullet and Blitz Play:** In faster formats, players often make moves that prioritize time management over board position. Traditional accuracy can't account for this, marking down players for rapid, time-saving moves.

- **Beginner Misrepresentation:** For newer players, the goal might not always be to play the best theoretical move but to set up familiar patterns or play aggressively. Traditional accuracy doesn't differentiate, potentially making their play seem worse than it is in a learning context.

- **Lacks Time Context:** Currently, the time left on a player's clock doesn't influence accuracy ratings. This means moves played with just seconds left are judged as harshly as those made with ample thinking time. This is especially relevant when players make moves that prioritize saving time over achieving the best position.

- **Narrative Limitations for Commentators:** For content creators and commentators, traditional accuracy can sometimes paint an incomplete or even misleading picture of the game. Crucial moments of drama, insight, or intuition are reduced to a numerical "inaccuracy" or "blunder."

- **Overemphasis on Theoretical Perfection:** A perfect game, in terms of traditional accuracy, doesn't necessarily reflect the nuances, challenges, or context of the match. Players might be penalized for trying new or unconventional strategies that the engine hasn't deeply analyzed.

- **Doesn't Account for Opponent Skill:** A move might be a blunder against a grandmaster but a brilliant play against a beginner. Traditional accuracy treats both scenarios the same, without adjusting for the opponent's potential responses.

- **Homogenization of Play Styles:** Strictly adhering to engine-approved moves, players might feel pressured to conform to a certain style of play, potentially stifling creativity or personal flair.

- **Coaching Conflicts:** From a coaching perspective, traditional accuracy might not always align with the advice or strategies a coach wishes to instill. It can be challenging to explain why an "inaccurate" move was the right practical decision in a specific situation.

</details>
<details>
<summary>🚀 Benefits of OA Accuracy</summary>
Bridge Between Theory & Practice: Understand where the ideal theoretical move and the best practical move diverge.

Training & Learning: Beginners can learn from comparing traditional and OA accuracies. Identify areas of reliance on tactics that might only work against certain player levels.

Narrative Creation: For content creators and commentators, both metrics offer a richer story of the game.

Future of Game Analysis: In an era of AI and machine learning, multiple metrics provide a deeper appreciation and understanding of human performance in chess.

</details>

<details>
<summary>💡 Potential Applications</summary>
Personal Game Review: Understand your playstyle, strengths, and areas to improve.

Chess Platforms: Offer users an additional metric for post-game analysis.

Streaming & Commentary: Enrich game discussions by highlighting instances where OA accuracy provides a different perspective from traditional accuracy.

</details>
Contribute & Feedback
Feel free to fork, raise issues, or submit pull requests. We value feedback from the community to refine and enhance OA Accuracy.
