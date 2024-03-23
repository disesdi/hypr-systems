-------

[home](https://mlops.archi/)  \| [about](https://hypr.systems/about.html) \| <a href="https://anglesofattack.io/" target="_blank" rel="noopener noreferrer">angles of attack</a>

-------

# Cutting Through the Hype: Three Things I Wish More People Understood About Real (Production) AI

### By <a href="https://mlops.archi/about.html" target="_blank" rel="noopener noreferrer">Disesdi</a> | 13 November 2023

-------

## Introduction: Defining & Mitigating the AI Hype Cycle

*The public AI conversation has gone off the rails*. 

That is the crux of conversations I am hearing in many AI ethics & MLOps spaces.

To a lot of AI/ML practitioners, the last year or so of AI discourse has been frustrating, bewildering, and at times, *exhausting*. 

The common complaint is that real issues in AI/ML are being ignored, while lawmakers and the public are fed a stream of non-information (hype) about science fiction-style future threats from all-powerful…robots, who are also inexplicably bent on the destruction of humanity. Or something.

Meanwhile, many of us in the field are facing (actual, real) dual crises of unethical misapplication of AI/ML tech, & unsecured, poorly-built and barely-productionized AI/ML systems in the wild.

After what I perceived as another egregiously bad AI hype cycle, it was getting to the point that turning on the news or scrolling through social media was becoming irritating, and the frustration wasn’t abating when I stayed out of the conversation, either.

While I definitely wish I could tackle all the misconceptions about AI out there right now, I am personally a fan of working towards the positive, rather than against something that’s negative. 

With that in mind, I decided that instead of starting out by countering everything misleading or false that I see in the news, my approach here would be to talk about some of the things I think people *should* pay attention to.

My hope is that those who are truly interested in how to build safe, secure AI systems that provide *actual business value* (hint: not hype), and do so in a way that organizations can actually implement, will take these informational points as a gateway to research the worlds of MLOps & MLSecOps.

So here are three things I wish more people understood about real, production AI — and, at the end, I’ll go over one area I see that’s actually *improving*.

## 1. Data in, predictions out

Getting business value out of models, regardless of their size or complexity, works on a simple principle: We use data to make inferences or predictions.

Another way to succinctly conceptualize this is *Data in, predictions out.*

This might seem straightforward, but the number of non-ML engineers I’ve had express appreciation for hearing it belies an importance that warrants further investigation.

What this hints at to me: Social literacy around AI/ML systems could perhaps be improved most rapidly through increased *data literacy.*

How this applies in industry: We make sure that data teams begin with a solid understanding of the *business value* they’re providing in a given application, and how the data itself supports this mission.

The importance of such a simple statement to stakeholders also suggests the potential for significant organizational benefit from keeping non-data focused teams in the loop on ML development.

One simple way to do this is to keep a recurring meeting on the calendar, where data teams showcase a particular aspect of AI/ML development—although this isn’t always possible with scheduling constraints, especially in a fast paced environment. 

Currently, our team uses Agile methodology & Scrum ceremonies to showcase and document our data work for the rest of the group. However, even a newsletter can be helpful for early stage teams looking to increase their cross-functional ML knowledge.

Even—or perhaps especially—if the message is a consistent reminder that everything begins with the data.

## 2. It Takes Very little code To Create production AI

The one aspect of artificial intelligence & machine learning engineering that surprises people outside the field the most consistently, in my experience, is *how little code* it actually takes to get even a relatively sophisticated model up and running.

What this code doesn’t do: test, monitor, retrain, or ensure that the model is sound & ethically applied.

Much of the heavy lifting when it comes to getting models into production isn’t coding a new, elite algorithm—it’s aligning business interests with data science capabilities, and creating policies that help make sure successes are both replicable, and sustainable. 

## 3. Some Of The Most interesting AI questions have nothing to do with “AGI”

So-called “Artificial General Intelligence” (AGI) is in the news lately as public interest in LLMs proliferates—but is this really the entire cutting edge of AI?

Evidence from the front lines says no. This is due to several factors:

LLMs require high experimentation time and massive compute to develop in-house; these resources simply are not available to many organizations.
Increasing evidence of security risks, liabilities, as well as practical issues of productionization limit ROI calculations for all types of LLM implementation
As in many cases, business value can often be achieved via novel application of existing machine learning techniques, often using free & open source AI/ML libraries.

As more and more practitioners realize the limitations of LLMs—security, safety, and even production-readiness—it makes sense that attention might shift to questions that get to the core aspects of practical, production-grade AI.

These include questions around a potential data crisis, nontheoretical productionization, and the intersection of ethical & secure AI.  

### What happens when we run out of data?

The impending [data crisis](https://www.technologyreview.com/2022/11/24/1063684/we-could-run-out-of-data-to-train-ai-language-programs/)<sup>[1]</sup> isn’t currently making the headlines that AGI or other scifi-esque “threats” are right now, but it [probably should be](https://www.newscientist.com/article/2353751-ai-chatbots-could-hit-a-ceiling-after-2026-as-training-data-runs-dry/): novel language data to train AI models is predicted by some measures to run out by 2026, because humans cannot produce it at a rate fast enough to outpace the models’ consumption.<sup>[2]</sup> 

The problem is serious enough that discourse included one AI CEO posting to social media what appeared to some to be [earnest plans](https://anglesofattack.io/4/data_hacking.html) to steal training data.<sup>[3]</sup>

### How do we ensure that our models make it into production—and work?

The [Google Practitioner’s Guide to MLOps](https://services.google.com/fh/files/misc/practitioners_guide_to_mlops_whitepaper.pdf) put it succinctly: 

*To summarize: models don’t make it into production, and if they do, they break because they fail to adapt to changes in the environment.*<sup>[4]</sup>

While productionizing remains a stumbling block for many organizations, it doesn’t have to be. In fact, we find that considerations around production scalability, ethics and security are complimentary. Secure & responsible AI go hand in hand; for our team, it all starts with MLOps.

With thoughtful planning, it’s possible to create pipelines that also provide increased security, and responsible AI—more on that below.

### How do we make sure our models don’t do harm?

Everyone says they want to build ethical AI. But as of very recently, doing so in practice remains elusive for many organizations.

While most practitioners seem to agree that audits are a good idea, there can be a marked lack of consensus when it comes to how, exactly, these should be implemented. 

The problem was so large that in 2022 I decided to design a [platform-agnostic secure MLSecOps system](https://anglesofattack.io/Securing_AIML_Systems_in_IW_Cox.pdf), with built-in auditing.<sup>[5]</sup> 

My goal was to demonstrate a practical implementation that could be adopted widely in industry, integrating both security and ethical AI into production. This architecture is the basis for much of what we are building on my team now.  

As the regulatory landscape around AI in production shifts, some organizations have been left scrambling to adapt to government and consumer expectations around ethical AI adoption. The goal is deceptively simple: *Don’t be one of them*.

### How do we secure AI?

AI security is a massive issue, with many different areas of research and applications. It’s also one of the AI/ML knowledge areas that I think is actually improving. Here’s why:

First, AI security awareness is increasing. From [high profile vulnerabilities](https://protectai.com/blog/hacking-ai-system-takeover-in-mlflow-strikes-again-and-again),<sup>[6]</sup> to a [growing body of papers](https://github.com/disesdi/mlsecops_references) in the field,<sup>[7]</sup> to an AI-focused village at [security conference DEFCON](https://www.nytimes.com/2023/08/16/technology/ai-defcon-hackers.html),<sup>[8]</sup> it’s becoming increasingly clear that AI security is an idea whose time has come.

As AI security enters more and more into the public & industry consciousness, we are likely to see both more high-profile attacks, as well as concerted efforts at advancing the state of the art for AI defensive security.  

Second, not only is AI security awareness increasing, but as it does so it breaks down the siloing of information that has kept machine learning and security practitioners largely separate—Until very recently. 

It’s not just a question of increased awareness or even the growing interest in the field for AI & ML security: because this area brings together two formerly disparate research areas, the potential for growth as collaboration increases is incredibly exciting. 

## Conclusion

AI hype can sometimes overshadow the real news in the field. I believe that as an engineer, if I can help to dispel some of the hype and fear, and contribute to the public being able to focus on real issues that advance the state of the art—that is a good thing. 

As an engineer, I look around and one thing is clear: from the data crisis, to the hunt for truly ethical AI, to the exciting world of AI security, the most interesting questions in AI aren’t the ones in the news. 

But they should be.

-------


### [Contact me >>](https://mlops.archi/about.html)


-------

## References


1. Xu, Tammy. 2022. “We could run out of data to train AI language programs.” MIT Technology Review. https://www.technologyreview.com/2022/11/24/1063684/we-could-run-out-of-data-to-train-ai-language-programs/.

2. Stokel, Chris. 2023. “AI chatbots could hit a ceiling after 2026 as training data runs dry.” New Scientist. https://www.newscientist.com/article/2353751-ai-chatbots-could-hit-a-ceiling-after-2026-as-training-data-runs-dry/.

3. Cox, Disesdi Susanna. 2023. “Did An AI CEO Just Tweet About Stealing Data?” Angles Of Attack. https://anglesofattack.io/4/data_hacking.html.

4. “Practitioners guide to MLOps: A framework for continuous delivery and automation of machine learning.” 2021. Google. https://services.google.com/fh/files/misc/practitioners_guide_to_mlops_whitepaper.pdf.

5. Cox, Susanna. 2022. “Securing AIML Systems in the Age of Information Warfare.” Angles of Attack. https://anglesofattack.io/Securing_AIML_Systems_in_IW_Cox.pdf.

6. McInerney, Dan. 2023. “Hacking AI: System Takeover in MLflow Strikes Again (And Again).” Protect AI. https://protectai.com/blog/hacking-ai-system-takeover-in-mlflow-strikes-again-and-again.

7. Cox, Disesdi Susanna. n.d. “MLSecOps Reference Repository.” GitHub. Accessed October, 2023. https://github.com/disesdi/mlsecops_references.

8. Hsu, Tiffany. 2023. “When Hackers Descended to Test A.I., They Found Flaws Aplenty.” The New York Times. https://www.nytimes.com/2023/08/16/technology/ai-defcon-hackers.html.
