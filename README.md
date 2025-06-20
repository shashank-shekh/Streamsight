# Streamsight: A Real-Time AI-Powered Community Intelligence Platform

## The Core Idea
In today's fast-paced digital landscape, the public conversation about a company and its products happens continuously across dozens of platforms. This unstructured feedback is a goldmine of actionable intelligence, but it's often lost in the noise. Streamsight is a real-time listening platform designed to solve this problem.

At its core, Streamsight ingests live data streams from developer-centric social platforms like Reddit, Twitter/X, and Hacker News. It then uses a sophisticated AI agent built with LangChain to analyze, enrich, and structure this data in real-time. The result is a live, centralized intelligence hub that transforms chaotic public chatter into a clear, prioritized, and actionable feed for multiple business departments.
The platform moves beyond simple keyword alerts. It understands the sentiment, classifies user intent, summarizes complex discussions, and identifies which products are being discussed and whether the user needs support.

## Business Impact:
A dashboard is the visible output, but the true value of Streamsight lies in its ability to drive proactive, data-driven decisions across the organization. For Product and Engineering, this means moving from slow feedback cycles to having real-time product insights, allowing for the immediate identification of bugs, feature requests, and competitor critiques. This transforms the product roadmap into a dynamic, instantly responsive asset. Simultaneously, Marketing and Brand Health teams gain a live pulse on brand perception, enabling them to measure the immediate impact of campaigns and identify community advocates. The system also empowers Sales and Lead Generation by functioning as an automated sourcing engine, identifying clear buying signals in public conversations and routing these high-quality leads directly to the sales team. Perhaps most immediately, Support and Developer Relations (DevRel) are transformed from a reactive to a proactive function. By automatically flagging users who are struggling, the DevRel team can engage before frustration builds, creating immense goodwill and cementing a reputation for world-class support.

## Role of AI:
1. Filtering out posts actually related to the target company. Reddit/Twitter searches are more of keyword based, using AI we are able to determine if the post is actually talking about the organisation or just the keyword
2. Finding intent of the posts, whether post is a support request, question, criticism, announcement or a general discussion
3. Overall sentiment
4. Real time top action items for the Company from the collected posts
5. Let support agents talk to AI agents about the posts and seek insights or questions


## Role of Confluent:
1. Schema Registry: Guardian of Data QualityPrevents garbage and malformed data, enable safe evolution and decouple components 
2. Elastic Search sink connector:Automates the data ingestion rather than us writing and maintaining our own ingestion pipeline. Supports the dashboard and search 
Streamsight is more than a social media dashboard; it is an automated intelligence engine that provides a strategic advantage. By leveraging a modern streaming architecture with Confluent at its core, it transforms unstructured, real-time public conversations into a high-fidelity signal that can drive product strategy, accelerate sales, and build a world-class customer support experience.

## Demo Screenshots

### Dashboard home page:
The top of the page shows a one liner executive summary, the top action items Organization can focus on, overall reliability score based ons ocial media pules, the sentiment pie chart, most talked about topics and also the latest posts
![Dashboard1](https://github.com/user-attachments/assets/a66bb2c7-781f-41fc-994c-73332a8638a9)

### Criticism + Support posts:
This filters out the posts that are criticizing the product and also the support requests so that they can be separately acted upon. Also lists a line chart of mentions over time
![Dashboard2](https://github.com/user-attachments/assets/814e3d16-edde-425f-856e-6c17d384d493)

### AI insights and conversation with post
Using an AI agent, this lets you have convesations with AI about the particular post. What the post is about, summary, insights, background, solutions....
![AI conversation](https://github.com/user-attachments/assets/b5b19338-5c13-4927-a9f0-8011a135803d)









