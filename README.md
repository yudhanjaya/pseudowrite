# Pseudowrite
Pseudowrite is a tool built as a demo for an Augsberg MFA panel that I was spoke at.
It will take a few lines of idea, and, using an iterate-refine loop, will turn it into a coherent act structure and chapter outline.
                    

https://github.com/yudhanjaya/pseudowrite/assets/16394240/00423dce-a87b-46be-8a88-7a700fdc880c


This tool is not, under any circumstances, to be used for any commercial purpose. Any use of this tool for commercial purposes is a copyright violation.
By using or modifying this tool you accept these conditions.


# A better introduction:
This is an exploration of what AI might do for writing. What initially began as a test of Sudowrite's "soup to nuts" claim
(result: meh) became an attempt at building a more stripped down story generator / assistant. 
It is neither a commercial product nor state of the art - I probably spent two-three days getting this to proof of concept,
and maybe another two days polishing it.

Many people think of these sorts of AI-for-storytelling devices as writing sentences for you, but this is a more plausible path: AI as a planner, as a cheap wayfinder,  especially for highly formulaic writing. If anything, the ease with which Psuedowrite, as simple as it is, can generate reasonably competent plots should be a warning: whatever can be made formulaic will, with or without AI, fall prey to various attempts to make it more efficient and more streamlined. 

The corpus of data underlying OpenAI's GPT models is unknown, and almost all current efforts - open source or not -
use a dataset called the Pile. The Pile contains BookCorpus2 and Bibliotik, 
two collections of books and stories that exist in violation of author copyrights.
My explorations of these datasets show everything from self-help books to LEGO Ninjago novels.
This is theft. 
            
At the same time, AI itself - in this case, the transformer architecture - is 
a fascinating and transformative device worth experimenting with; certainly one that will 
have to be reckoned with.
                    
If you are considering the use of AI in fiction, first learn the fundamentals of the craft.
Otherwise, even if an AI model writes the Next Great Novel, you will not be able to discern good from bad.
Read up on the history of procedural generation, NanoGenMo, as well as generative techniques in
literature to understand what you're getting into.
                   
Also see my 2018 story "The Writing Contest," as well as subsequent work with other writers and Google Research 
evaluating their LaMDA model for storytelling.

If this doesn't convince you, consider the US Copyright Office decision on AI-generated art:
                    
Reuters: "Zarya of the Dawn" author Kris Kashtanova is entitled to a copyright for the parts of the book Kashtanova wrote and arranged, 
but not for the images produced by Midjourney, the office said in its letter.
                    
                    
See: 
1. Gao, L., Biderman, S., Black, S., Golding, L., Hoppe, T., Foster, C., ... & Leahy, C. (2020). The pile: An 800gb dataset of diverse text for language modeling. arXiv preprint arXiv:2101.00027.
2. https://fingfx.thomsonreuters.com/gfx/legaldocs/klpygnkyrpg/AI%20COPYRIGHT%20decision.pdf
3. https://yudhanjaya.com/The-Writing-Contest-824fdd034b9e467f8747f04e3d1de44d
4. https://g.co/research/wordcraft
                    
# How does this work?
Pseudowrite uses OpenAI GPT 3.5 and GPT 4 and the concept of outlining to take an idea from basic notes to chapters. We use a constant derive-> refine loop to iteratively feed the AI specific commands. 
        
At any point, you are free to also edit the text given to the AI so you have more control over the outputs. 

There are three stages of operation: 
First stage: you put down your ideas in the form of rough idea, story and characters.
You use the refine options to iterate on whatever's in that box.

Second stage: you derive an act structure from the ideas in the first stage. 
This will also give the underlying story. You can refine this as well, or take a more hands-on approach.
Either way, when you're satisfied, move onto the third stage.

Third stage: we derive chapter notes from the acts above. By now you should be fairly happy with the story.
If you need to make changes, tweak the text by hand. 
        

# Why do you do it this way?
Because AI isn't all-intelligent just yet. 
Right now, the large language models (LLMs) have attention limits. A simple explanation is that they can only 'see' so many characters at a time, and they can also only output so many characters. A more complex explanation is that even with expanded context windows, most LLMs 
Therefore, iterative tweaking - known as Chain-of-Thought - is how we get AI to do complex things. \n
While I myself do not use this style of extensive outlining, many successful authors do: see the Snowflake pattern of writing, Save The Cat, or Brandon Sanderson's approach. 
It is also useful for learning.
        
It is, however, nowhere near as competent yet as an author with knowledge of their craft.""")

# What is the Playground?

The playground is a replica of OpenAI's Playground, where you can directly command the model.
For example, you can say 'read the paragraph below this and rewrite it as a poem'. 
To better understand how to do this, read: https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api

 # Version history

        \n Version 0.6: Public version, code cleaned up
        \n Version 0.5: Structure -> Chapter flow reworked, added Playground and Help.
        \n Version 0.4: Reworked visuals, added new theme, first testing and evaluation.
        \n Version 0.3: Genre-based AI personalities added. Code refactored.
        \n Version 0.2: Rearchitected around derive-> refine loop
        \n Version 0.1: Janky replica of Sudowrite's story engine
