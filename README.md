# Shoulder-Abduction-in-Hitting
Hi everyone, I wanted to share some work I've done these past few months.


I was trying to find new problems to solve using Driveline Baseball's OpenBioMechanics data. I found a Driveline article about how they considered changing one of their pitchers' shoulder abductions.

It was interesting because they used the shoulder abduction angle to indicate change. They were not specifically trying to change that measure, rather they looked at the change in shoulder abduction as a product of improving the pitcher's arm movement efficiency.

They do this by creating a custom custom training plan with specific drills. Here's the link to the article:


https://www.drivelinebaseball.com/2018/12/changing-shoulder-abduction/


With my curiosity for hitting research, I thought of how I could try to look at shoulder abduction for hitting (particularly the rear shoulder).

I thought of the concept of 'loading the scap' in hitting, where you'd want to 'pull back' your elbow when loading. I also thought of how some coaches would tell kids to not 'chicken wing' their elbow when thinking about shoulder abduction.

My goal was to find out if what Driveline did on shoulder abduction and pitching can also be implemented in hitting. In this case, I want to try to correlate the rear shoulder angle in the 'y' direction with bat speed (instead of looking at pitch velocity).

So I loaded the data, did a little bit of cleaning for missing values, and then I started simple using a normal linear regression model to see if a linear relationship exists. I looked at the summary statistics and plotted the model. The summary statistics and graph are in the repo.

With the R^2 score being low (0.01), we can suggest that there isn't a linear relationship between the shoulder angle and bat speed. But, the graph tells us here that most of the swings happen between 60-90° and they sit between 65-75 mph.

The higher bat speed values (>80) are also between 70-105°. Regardless, this still suggests that shoulder abduction has a weak correlation to bat speed. But then I thought of how the pitching study I mentioned before focuses on the shoulder abduction at around 90°.

I realized that the model above predicts a linear relationship between bat speed and shoulder abduction. My original goal was to see specifically if keeping your shoulder abducted at 90°correlates with high bat speed. I decided to change my model-building approach.

I realized that the model above predicts a linear relationship between bat speed and shoulder abduction. My original goal was to see specifically if keeping your shoulder abducted at 90°correlates with high bat speed. I decided to change my model-building approach. The summary statistics and graph are in the repo.

We did see an increase in the R^2 value to 0.02, but it still signifies a weak correlation. What's interesting in the graph though is that most of the swings take place within 10° of 90, so we can say that athletes usually have their shoulders around 80-100° max before footplant.

Nevertheless, I can't conclude that shoulder abduction directly affects bat speed. But I still think it's an important thing to consider when training a swing. The previous graph shows that in the 30-40° difference, the bat speed sits below 65 mph.

This means that it may be tougher for someone to get a higher bat speed when they have their rear shoulder abducted too high or low. So when assessing hitters, shoulder abduction should still be something to look out for. 

It's just not a defining factor for hitters with fast bat speeds. We should just look at whether the athlete is staying around the 0-20° degrees from 90°. That's one thing I can take away from this analysis. I think that one body part can't help increase bat speed. 

Just like in the pitching analysis Driveline did, they saw a decrease in shoulder abduction angle in the athlete because of a lower trunk positioning and tilt angle. They did this by implementing drills to help the athlete move more efficiently.

I think the same can be applied to hitting. We should train to move efficiently when swinging, and I can say that through this study the rear shoulder abduction is just 'one piece of the puzzle' when it comes to creating an efficient swing. 

Therefore, rear shoulder abduction in a swing doesn't correlate strongly with bat speed but can be a good indicator of someone moving efficiently throughout a swing. And like pitching, there is more to be studied in hitting and swinging movements. 

Some things I can do moving forward is to further study each swing of the data to see how the rear shoulder moves over time. I can also explore other relationships between bat speed and other key body parts in hitting. 

Either way, I'm glad I investigated this topic and I hope you enjoyed reading my analysis! I hope to keep trying to uncover more baseball problems and contribute to the baseball development world!

I also appreciate any feedback that y'all can give me. I want to be better at posting threads and my work. It's a way for me to practice being a baseball researcher. Please don't hesitate to comment or contact me.

