# Problematic:
I need to calculate, for a specific user, the probability of buying at least one product from subfamily -4829876793851668777 during the next 14 days.

Since we don't have information, I assume that we are trying to calculate this value for a future date in 2024 (available data 2021, 2022, 2023), left to the user's choice.


To undertake this exercise, two approaches could be considered: taking into account the past consumption history or considering the user profile.

The second option appeared to me to be the most relevant for this type of problem (I will come back to it later). But I prefer to work on historical analysis.

The reasons are:
* There are not enough indications about the various information present (different columns of the dataset), and I do not know how they are correlated.     For example, are there more sales in this store_id because the store is larger, or is there simply more people around (confounding factor)?
*  To create  user profile we need information like gender age, profession (what we don't have here, excepted gender)
* It does not answer the question of estimating for a user (who is characterized by their purchasing profile historics rather than their group).

My analysis will therefore focus on past consumption analysis to answer the question.

However:
In the case of the subfamily -4829876793851668777, as we will see later, purchases are very localized and punctual, which makes historical analysis comparatively much less reliable than an analysis based on the user's profile.