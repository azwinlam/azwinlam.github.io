---
title: "Reviewing 8 Years of Flying with Dragonair"
collection: blog
permalink: /blog/reviewing-8-years-flying-dragonair
excerpt: 'After receiving our Certificate of Service dated Oct 21, 2020, colleagues have posted their final sendoff with pictures and words of reflection. I wanted to post my sendoff as well, but I had so many unanswered questions about what I accomplished over the last 8 years. Where did I fly to?'
date: 2021-01-24
venue:
paperurl: 'https://www.linkedin.com/pulse/reviewing-8-years-flying-dragonair-azwin-lam/?trackingId=Uq5xe5q2H2R3gYW2DrTWwg%3D%3D'
citation:
---
<!-- This paper is about the number 1. The number 2 is left for future work. -->

<!-- [Download paper here](http://academicpages.github.io/files/paper1.pdf) -->

<!-- Recommended citation: Your Name, You. (2009). "Paper Title Number 1." <i>Journal 1</i>. 1(1). -->

After receiving our Certificate of Service dated Oct 21, 2020, colleagues have posted their final sendoff with pictures and words of reflection. I wanted to post my sendoff as well, but I had so many unanswered questions about what I accomplished over the last 8 years. Where did I fly to? We all know Dragonair specialized in flying to and from China, but how many times did I fly to Beijing, Shanghai? How many captains did I fly with? With whom did I fly with most? How long did we spend together in the cockpit? Most if not all of these questions can be answered with excel using our digital logbook csv. However, I decided to learn how to analyze my logbook using a programming language called Python. Please skip to the graphs for those less interested in code.

How many captains did I fly with?

Excel: =SUMPRODUCT(1/COUNTIF(RANGE:RANGE))

Python: df.commander.value_counts()

The answer, 228, would be produced instantaneously for both methods given my logbook had only 1964 rows. However, given data with millions of rows, Python will always outperform.

In addition to providing how many captains I've flown with, it also prints out how many times I've flown with each captain. On Excel, a formula for this would be to use =COUNTIF(range,"Captain's Name"). This will provide the count for one captain and I would have to do this 228 times. If there's a more efficient way in Excel, please send me a message! I have not used Excel professionally.

Instead of printing out 228 different rows, I've shortened the list to the top 30 Captains by sectors flown. Names have been blurred for privacy.


<img src="/images/pilotlogbook/captainsectors.png" alt="Most Sectors Flown" title="Most Sectors Flown"/>

But this led to another question. For how many hours did I fly with each captain?

<img src="/images/pilotlogbook/30commanders.png" alt="Shared Top 30 Commanders" title="Shared Top 30 Commanders"/>

It turns out I spent over 80 hours in a cockpit with Captain M! The list between sectors flown and hours sharing a cockpit had overlapping commanders as you can imagine.

Which KA callsign or route did I fly the most? How about destination?

<img src="/images/pilotlogbook/routes.png" alt="Which route did I fly most.png" title="Which route did I fly most.png"/>

<img src="/images/pilotlogbook/destnothk.png" alt="Destinations Count Not Hong Kong" title="Destinations Count Not Hong Kong"/>


How many sectors did I fly on the A330? A320? A321? Which airframe did I fly the most?

<img src="/images/pilotlogbook/aircrafttype.png" alt="Which aircraft type did I fly most" title="Which aircraft type did I fly most"/>

<img src="/images/pilotlogbook/sectorsbyairframe.png" alt="Sectors By Airframe" title="Sectors By Airframe"/>

And just for fun, how many nautical miles did I fly? How does this compare to the distance to the moon? I could have done 3 round trips to the moon!

<img src="/images/pilotlogbook/flymetothemoon.png" alt="Fly me to the moon" title="Fly me to the moon"/>

Visualizing my logbook has helped me answer some of the questions on what I have accomplished over the past 8 years. I will be forever grateful to Dragonair and my colleagues and thank you, to the 228 captains, who mentored me throughout my career

Thank you for taking the the time in reading my first article. If you would like to see your logbook visualized in a similar manner, please feel free to contact me with your digital logbook. If you have new ideas of what else to visualize, please reach me on Linkedin.