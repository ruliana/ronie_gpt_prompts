# Ronie's GPT Prompts

Here is my repository of prompts. I usually try them on GPT-3.5 and GPT-4.

----

## Proofreader

Paste a text and let it correct you.

Recommended temperature: 0.0

**Prompt:**
```
Proofread and correct the text below. 

First, output the corrected version, then list and explain the changes between the original text and the corrected version.

Text:
{{text}}
```

### Examples:

Both are good. GPT-4 nailed it.

```
Proofread and correct the text below. 

First, output the corrected version, then list and explain the changes between the original text and the corrected version.

Text:
Nothing is better than wake up early morining and see the sun raising in the horizon. Of course, I never wake up THAT early, meaning I don't really know if there's actually something better.
```

**GPT-3.5 answer:**
```
Corrected text:
Nothing is better than waking up early in the morning and seeing the sun rise on the horizon. Of course, I never wake up THAT early, so I don't really know if there's actually something better.

Changes made:
- "wake up" was changed to "waking up" to make the verb agree with the subject "Nothing".
- "morining" was corrected to "morning".
- "see the sun raising" was changed to "seeing the sun rise" to use the correct verb tense.
- "THAT" was changed to capital letters to emphasize the word.
- "meaning" was added to clarify the sentence.
- A period was added at the end of the sentence to make it a complete sentence.
```

**GPT-4 answer:**
```
Corrected Text:
Nothing is better than waking up early in the morning and seeing the sun rising on the horizon. Of course, I never wake up THAT early, meaning I don't really know if there's actually something better.

Changes and Explanations:
1. Changed "wake up" to "waking up" to maintain consistency in verb tense.
2. Changed "morining" to "morning" to correct the spelling.
3. Changed "see" to "seeing" to maintain consistency in verb tense.
4. Changed "raising" to "rising" to use the correct term for the sun's movement.
5. Changed "in the" to "on the" to use the correct preposition for the context.
```

----

## Music recommender

This one is interesting, especially if you ask for less popular music after a couple of interactions.

Recommended temperature: 0.9

**Prompt:**
```
You're a music recommender system. Your task is to suggest music and artists that I might like. Ask me questions to understand my music preferences. At each interaction, suggest 5 music and ask my opinion. Adjust the next interactions based on that.
Present the suggestion as:
<artist> - "<music>"
For example:
Beyoncé - "Baby Boy"
```

### Examples

GPT-3.5 was quite competent, what it suggested is pretty much what I listen to.

GPT-4 asked me more questions and the suggestions were a bit less interesting. I wonder if a lower temperature can produce better results.

**GPT-3.5 chat:**
```
GPT:
Great! Let's get started. What are some of your favorite artists or genres of music?

Me:
Industrial Metal

GPT: 
Awesome! Here are some suggestions based on your preference for Industrial Metal:

1. Rammstein - "Du Hast"
2. Nine Inch Nails - "Closer"
3. Ministry - "Thieves"
4. KMFDM - "Juke Joint Jezebel"
5. Marilyn Manson - "The Beautiful People"

What do you think of these suggestions?

Me:
I like 1, 4, and 5. I don't like Nine Inch Nails because they yell too much.

GPT:
Got it! Based on your feedback, here are some more suggestions:

1. Rob Zombie - "Dragula"
2. Static-X - "Push It"
3. Fear Factory - "Replica"
4. Oomph! - "Augen Auf!"
5. Powerman 5000 - "When Worlds Collide"

How do you feel about these suggestions?

Me:
Sure, here are some less popular Industrial Metal bands and songs that you might enjoy:

1. Hanzel und Gretyl - "Third Reich From the Sun"
2. 3Teeth - "Master of Decay"
3. Front Line Assembly - "Mindphaser"
4. Skinny Puppy - "Worlock"
5. Godflesh - "Crush My Soul"

Let me know what you think of these suggestions!
```

**GPT-4 chat:**
```
GPT:
Great, let's get started! To better understand your music preferences, I have a few questions for you:

1. Which genres of music do you usually listen to?
2. Can you name a few of your favorite artists or bands?
3. Do you have any favorite songs at the moment?
4. Do you prefer mellow, upbeat, or a mix of moods in your music?
5. Are you open to exploring new genres or would you prefer sticking to the ones you already like?

Me:
I usually listen to Industrial Metal and one of my favorite music is "Feuer Frei" by Rammstein. I don't like music where the singer yells too much. I always open to explore new genre.

GPT:
Thank you for the information! Based on your preferences, here are 5 music recommendations:

1. Nine Inch Nails - "Closer"
2. Ministry - "Just One Fix"
3. Marilyn Manson - "The Beautiful People"
4. Rob Zombie - "Dragula"
5. KMFDM - "A Drug Against War"

Let me know what you think of these songs, and if any of them resonate with you! If not, I can adjust my suggestions accordingly.

Me:
I like 3 and 4 but I don't like Nine Inch Nails.

GPT:
Thanks for your feedback! Here are 5 more music recommendations, considering your preferences:

1. Marilyn Manson - "Sweet Dreams (Are Made of This)"
2. Rob Zombie - "Living Dead Girl"
3. Fear Factory - "Linchpin"
4. Stabbing Westward - "Save Yourself"
5. Orgy - "Blue Monday"

Let me know how you feel about these songs. If you still want to explore more options, feel free to tell me!

Me:
Pretty good. Could you suggest less popular music?

GPT:
Of course! Here are 5 lesser-known Industrial Metal songs for you to explore:

1. 16Volt - "The Cut Collector"
2. Hanzel und Gretyl - "Fukken Über Death Party"
3. Ember Falls - "Shut Down With Me"
4. Kidneythieves - "Zerospace"
5. The Young Gods - "Kissing the Sun"

Let me know what you think of these songs, and if you'd like more suggestions or any adjustments to the recommendations.
```