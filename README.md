# SMI-FinalProj-TruthSocialPlatformStudy

I use mostly R to do my analysis.  
Please refer to the code in Rproj/TruthSocialAnalysis.Rmd for most of my work.  

Truth Social Dataset paper: Data Schema of the whole dataset.  
![image](https://github.com/josephj1o4e1/Truth-Social-Platform-Study/assets/13396370/3682df86-50d8-4968-b2d0-ace45846fb31)  
  
Top 20 hashtags.  
![image](https://github.com/josephj1o4e1/Truth-Social-Platform-Study/assets/13396370/e4656752-a18c-45e5-8504-cbf61a4fd341)  
  
Top 20 Retruthed Users.  
![image](https://github.com/josephj1o4e1/Truth-Social-Platform-Study/assets/13396370/40b570d4-8193-4204-9ed9-425097643085)  
  
The Degree Distribution is Power law shaped.  
![image](https://github.com/josephj1o4e1/Truth-Social-Platform-Study/assets/13396370/bf79a25e-c104-49a0-9a4d-aa6a37326331)  
  
Top 20 Hubs in the Network.  
![image](https://github.com/josephj1o4e1/Truth-Social-Platform-Study/assets/13396370/a4c7b12d-4727-448a-9b23-7ca13b4c4954)
  
Keyword spike analysis from the paper.  
![image](https://github.com/josephj1o4e1/Truth-Social-Platform-Study/assets/13396370/1041d427-6e11-4d6f-8134-4ac8d7c0a382)


By looking at the top hashtags, retruthed users, and Hubs, we can reasonably suspect that the Truth Social platform is highly manipulated in
favor of Donald Trump and his supporters.  
Despite all these obvious results, I would like to throw out some questions.  
If we want to strongly claim the responsibility of Truth Social or its related platforms, public figures, I think there are more things to be confirmed.  

Discussion 1:  
In the Truth Social Dataset paper (P. Gerard, 2023), the author also did some interesting analysis and visualizations. In the trend graph (Feb 2022 ~ Oct 2022) indicating the Keyword spikes of “Jan 6 Capitol Riots” and “FBI Mar-a-lago”, the authors reveals that the spikes in Truth Social symmetrically matches the spikes in Google Trend.  Thus, it is suspicious that the platform is suspicious for provoking such contents at the time.  
However, just by looking at the trend spikes of frequency count of posts is not enough to claim that Truth Social is responsible and is more dangerous than other platforms. 
Mainstream platforms might also have similar spikes around the time of certain events. Maybe we should further ask:  
•	Is the proportion of the “keyword related truths” to “all truths” higher compared to other mainstream platforms?  
•	Are there any odd behaviors from “responsible users”  
    Responsible users: Hubs and its community within path length < 3  
•	Content Analysis:  Are there more provoking contents? How should we define the content as ‘provoking’?  
•	Which user accounts are responsible for those provoking contents?  
•	Are the chances higher for a user to encounter these provoking contents?  
•	Are the provoking contents false?  
  
Discussion 2:  
Does the dataset still have sampling bias? The author reveals that they did a bread-first manner scraping staring from @realDonaldTrump. It would be intuitive to suspect that the data is biased.  
The author claims that the dataset is representable because the network has a short average path length, which is a key trait of a Watts and Strogatz network model (Watts, 1998) and BA network model (Albert, 2002).  
However, the Watts and Strogatz network model also suggest that networks have high cluster coefficients.  
Research has also shown that real-world networks are often sparse (Leskovec, 2008).  
Therefore, we should further test out the the cluster coefficients and the sparsity of the network to have a stronger confirm that the network from the truth social dataset is a real-world network.  

Discussion 3:   
According to this news post from The Hill (Klar, 2023), there is a possibility that after Parler was released again from the Capitol Riot ban,  
it is modifying its business model in contrast of its previous version.  
I suspect that there is a possibility where Parler users are switching to other platforms such as Truth Social.  
We can analyze the similar user conversion flow, and construct a Dual-Layered map visualization.  

