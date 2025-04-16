---
created: 2025-04-16 08:50
---
tags:: [[🗒️ Daily Notes]]

# Wednesday, April 16, 2025

<< [[Timestamps/2025/04-April/2025-04-15-Tuesday|Yesterday]] | [[Timestamps/2025/04-April/2025-04-17-Thursday|Tomorrow]] >>

---
### 📅 Daily Questions
##### 🌜 Last night, after work, I...
- Finished the exam quiz for financial module 3
- In unity:
	- Added animation for player: Run, Jump, Fall, Idle
	- Added flip player sprite to flip
```csharp
If (PlayerHasHorizontalSpeed())
	{
		animation.localScale = new Vector2(Mathf.Sign(myRigidBody2d.LinearVelocity.x), 1f);
	}
```


- Mathf.Sign is a math that tell direction based on number whether positive or negative (this will be better for 2d as you will not need Vector3 for transform)
- Mathf.Sign is great for determining **direction only**, not magnitude. Super useful for flipping sprites or controlling movement logic.
	- In order to tackle edge case preventing player from flipping sprite while not moving ~ 0.01f, PlayerHasHorizontalSpeed has to check and round up the number to be
```csharp
bool PlayerHasHorizontalSpeed() 
	{ 
		return Mathf.Abs(myRigidBody2D.linearVelocityX) > Mathf.Epsilon; 
	}
```
##### 🙌 One thing I'm excited about right now is...
- Continue backlog
- Continue Unity
- Research gtm plan
- Publish this Obsidian

##### 🚀 One+ thing I plan to accomplish today is...
- [ ] Finish parsing url
- [ ] Finish player unity

##### 👎 One thing I'm struggling with today is...
- Research gtm plan

---
# 📝 Notes
- 

---
### Notes created today
```dataview
List FROM "" WHERE file.cday = date("2025-04-16") SORT file.ctime asc
```

### Notes last touched today
```dataview
List FROM "" WHERE file.mday = date("2025-04-16") SORT file.mtime asc
```