# EventStorming Glossary & Cheat sheet

EventStorming is the smartest approach to collaborate beyond silo boundaries. The power of EventStorming comes from a diverse multi-disciplined group of people who, together, have a lot of wisdom and knowledge. While it originally was invented for a workshop to model domain-driven design aggregates, it now has a broader spectrum. From gaining a big-picture problem space of the whole domain to gaining insight into the entire software delivery flow and creating a long term planning. Every one of these workshops has the same basic requirements and needs. 

Here you will find a combination of a glossary of terms on EventStorming core concepts written down in a consistent and comprehensive glossary. Just be sure to try and avoid jargon as much as possible, as it sets up the unnecessary insider-outsider distinction. And a Cheat sheet that you can use facilitating your own EventStorming.

## Glossary

### Core Concepts

**Domain Event**
A Domain Event is the main concept of EventStorming. It is an event that is relevant for the domain experts and contextual for the domain that is being explored. A Domain Event is a verb at the past tense. The official EventStorming colour is orange.

**HotSpot**
Hotspots are used to visualise and capture hot conflicts. Conflicts caused by, and not exclusive to, inconsistencies (in language), frictions, questions, dissent, objections, issues or procrastinating going deep to explore for later. The official EventStorming colour is neon pink and we also slightly pivot a hotspot when we use it.

**Timeline**
EventStorming is a powerful tool when we have a story to tell, when we have a timeline. The paper roll on the wall represents time from left to right. We can have parallel streams from top to bottom on the paper roll.

![Core Concepts](/_resources/core-concepts.jpg)

**Chaotic Exploration**  
Chaotic exploration can be used at the start of EventStorming. Each person writes Domain Events by themselves that they can think off. They will put these Domain Events in order they think they happen on the paper roll.

**Enforce the Timeline**  
A phase happening after chaotic exploration, meaning we try to make the timeline consistent and remove duplicate stickies.

### Big Picture EventStorming

The goal of Big Picture EventStorming is to assess the health of an existing line of business or explore the viability of a new startup business model. It helps the group create a shared state of mind of the vision of that domain of the company. We can use the output as input for Conway’s law alignment, organising business flow around teams and software with emergent bounded contexts. You can do these workshop with 10-30+ people on one paper roll.

![Example big picture](/_resources/big-picture.jpg)

**Opportunity**  
Because a Hotspot can have a negative association we also give people the chance to add opportunities. We use green because of the association it has with something positive. Start using Opportunities after we made a consistent timeline.

**Actor/Agent**  
Actor or Agent is a group of people, a department, a team or a specific person involved around a (group of) Domain Event(s). The official colour to use is a small yellow post-it.

**System**  
A system is a deployable IT System used as a solution for a problem in the domain. When we have finished making the timeline consistent, we can start mapping systems around Domain Events. There can also be duplicates and it can be anything from using Excel to some microservice. The official colour is a wide pink post-it.

**Value**  
We can add value like we would do in a value stream map, after we have made the timeline consistent. We do this to make explicit where the value is in our domain. We use the red and green small stickies to show positive and negative value.

**Pivotal Events**  
With Pivotal Events, we start looking for the few most significant events in the flow. For an e-commerce website, they might look like “Article Added to Catalogue”, “Order Placed”, “Order Shipped”, “Payment Received” and “Order Delivered”. These are often the events with the highest number of people interested. 

![Pivotal Events](/_resources/pivotal-events.PNG)
*Source: https://leanpub.com/ddd_first_15_years – Discovering Bounded Contexts with EventStorming — Alberto Brandolini*

**Swimlanes**   
Separating the whole flow into horizontal swimlanes, assigned to given actors or departments, is another tempting option since it improves readability. This seems the most obvious choice for people with a background in process modelling.

![Boundaries](/_resources/boundaries.PNG)
*Source: https://leanpub.com/ddd_first_15_years – Discovering Bounded Contexts with EventStorming — Alberto Brandolini*

![Big picture tools](/_resources/big-picture-tools.jpg)

**Emerging Bounded Contexts**  
From a Big Picture EventStorming we can picture Emerging Bounded Contexts. They are the first indicators of where to start deep-diving towards designing bounded contexts around business problems.

![Emergent bounded context](/_resources/emergent-bounded-contexts.PNG)
*Source: https://leanpub.com/ddd_first_15_years – Discovering Bounded Contexts with EventStorming — Alberto Brandolini*

![Big picture legend](/_resources/big-picture-legend.jpg)

### Process modelling EventStorming

The goal of process modelling EventStorming is to assess the health of a current process in the company. It helps the group create a shared state of mind of the current status quo of the process, find bottlenecks and identify parts of the system to decouple from the existing software.

![Process modelling](/_resources/process-modelling.PNG)
*Source: https://leanpub.com/introducing_eventstorming*

**Policy**  
A policy is a reaction that says “whenever X happens, we do Y”, eventually ending up with in the flow between a Domain Event and a Command/action. We use a big lilac post-it for these. A policy can be an automated process or manual. A policy can also be named a reactor, eventual business constraint or rule or a lie detector because there is always more to policies than you first think.

**Command/Action**  
Represents decisions, actions or intent. They can be initiated by an actor or from an automated process. During process EventStorming usually, the word "Action" usually fits better with stakeholders than command because it is easier to grasp. We officially use a blue coloured post-it for it.

**Query Model/Information**  
To make decisions an actor might need information, we capture these in a Query Model. For process EventStorming information might be more recognised by stakeholders. We officially use a green post-it to represent a query model.

![Process design tools](/_resources/process-design.jpg)

**Enforce colour coding**  
Enforcing the colour coding is playing EventStorming by the rules. Often used after or during enforcing the timeline it creates a different dynamic. Below you see the colour coding and how they are to be used in the flow of the timeline. 

![Process picture](/_resources/process-picture.jpg)

### Software Design EventStorming

The outcome of a design level EventStorming is to design clean and maintainable Event-Driven software, to support rapidly evolving businesses. Together with business stakeholders, we design a shared language and represent that in a shared model that brings value in solving a problem within a bounded context.

**Constraint**  
A constraint is a restriction we have or need to design from our problem space when we want to perform a command/action, another word could be consistent business constraint or rule. The official color to use is a big yellow post-it. It was called an aggregate before which is now officially a legacy word in EventStorming, since we prefer not to use the word aggregate with business stakeholders.

![Software picture](/_resources/software-picture.jpg)
![Software design tools](/_resources/software-design.jpg)

## Cheat Sheet

### Preparations

#### Invites

Invites are essential to make it a successful workshop. You want to invite everyone who brings knowledge and who needs the knowledge, usually domain experts and the engineers. You want to add information about what the goal of the workshop is, and what EventStorming is. I always send the video Alberto Brandolini – 50,000 Orange Stickies Later to the attendees plus the resources page from eventstorming.com.

#### Materials

There is nothing so annoying as not having the right material, so you want to make absolutely sure you have everything needed. I have written a blog post here about it, go check it out!

#### Room setup

The best picture still is the one from the book EventStorming on leanpub. The idea is to have a modelling surface around 6-8 meters, a table for putting the materials on and a visible legend for people to see. We want to have no seats in sight. Also, you want a room preferable where the windows can open so you can have fresh oxygen in the room and have some food or candies lying around.

![Room setup](/_resources/room-setup.png)
*Source: https://leanpub.com/introducing_eventstorming*

#### Facilitation

For an effective EventStorming workshop, you want to have a dedicated facilitator.

As a facilitator:

* You want to have a neutral role so that you can cut long discussions short and visualise them with hotspots.
* You need to find to balance to when you will intervene and when you will let the discussion flow.
* You are always the first in the room and the last to leave, so you can set up the room correctly and talk with people afterwards.
* It is your job to facilitate the group and give them feedback and insights about the group interaction so that they can decide what to do. For instance, when you see multiple people looking on their phone, you can tell “I see that part of the group is distracted from the activity by looking on their phones”.
* You have to observe and let the group figure out what their needs are, however sometimes you need to decide for them when the group can’t.

### Workshop process

#### Check-in

I always start a workshop with what is called a check-in. It is essential to be present physically and mentally for the workshop. So in a check-in, ask the attendees questions about how it is going with them. Like how was their weekend, how are they feeling, what do they hope to get out of the workshop today. You must not discuss any workshop or work-related stories. Always check-in first as a facilitator and lead by example by sharing just enough. Afterwards, let participants in the group decide for themselves when they will check-in popcorn style! When everyone is done, it is important to wrap up and summarise as a facilitator what you heard the participants say.

##### Agreements

Because we have a room full of people with different perspectives, it is vital to make some agreements on how we collaborate during the workshop. We want to make it explicit by writing this on a flip chart and stick it to a wall so that you as a facilitator can point to these explicitly. I write and discuss the following three agreements from Deep Democracy:

* Everyone is right; nobody has the monopoly on the truth.
* We start a conversation to deepen our relationship.
* We are willing to learn together.

After you can discuss with the attendees if they themselves have rules they want to add and discuss these with them if they need to be added.

##### EventStorming

Now it is time to give an intro on EventStorming. I usually tell a microstory to the people explaining why classic forms of collaboration don’t work for me, and why EventStorming is different. These are personal and I advice you to figure out such a story for yourself. Explain the basics of what a domain event is on the legend.

![Domain Event](/_resources/domain-event.png)
*Source: https://leanpub.com/introducing_eventstorming*

**Step 1: Chaotic exploration**
Start with asking people to write their domain events that they know of for themselves. Here people must work by themselves so that we don’t bias each other. Also, try to avoid answering questions at this point. Tell them that they can put their domain events on the paper the way they feel is correct. We want their perception on the paper. Do not rush this part; this is the essential part of the whole EventStorming. When people start putting their domain events on they can begin to read each other’s events, but make sure they don’t begin discussing them out loud; it can bias or rush the others.

![Start EventStorming](/_resources/start-es.png)
*Source: https://leanpub.com/introducing_eventstorming*

**Step 2:  Enforce the timeline**
After you are sure everyone is done with putting their domain events on the paper, we can start enforcing the timeline. It means asking the attendees to:

* Start discussing the events, I expect a lot of noise and chaos now.
* Removing duplicate events, let them discuss if they really are duplicate events, it might be the same language for different concepts.
* Ordering all events in the correct timeline.
* Adding structure with tape when needed, but be careful adding structure too soon. You can lose valuable insights from doing so.

**Step 3: Hotspots**
During Step 2 we will get a lot of conflicts between several perceptions, which is good. Out of conflict we grow and gain new insights. However, to be able to manage these conflict we add a pinkish sticky where there are conflicts. We call these hotspots. Hotspots can also mean pain points or questions that are unanswered. As a facilitator, you at this phase add the hotspots.

**Step 4: Add concepts when needed**
Whenever another EventStorming concept pop-up, we add them to the legend and introduce these to the group. The picture that explains “almost” everything are the concepts you can add:

![Software picture](/_resources/software-picture.jpg)

##### Check-out

Like the check-in, we also want to end a workshop with a check-out. Stand in a circle with everyone and ask them what their thought was about the workshop. People can step inside the circle, give a statement and if other people agree they step with them inside the circle. Finish when you are sure everyone is done.

Remember, Alberto calls EventStorming like a pizza. The paper roll and domain events are the base of your pizza, the dough, but you put your ingredients on top of it the way you like it (as long as it isn’t pineapple 😉). 

## Sources

* [EventStorming.com](https://EventStorming.com)
* [Leanpub: Introducing EventStorming](https://leanpub.com/introducing_eventstorming)
* [Leanpub: DDD First 15 years](https://leanpub.com/ddd_first_15_years) – Discovering Bounded Contexts with EventStorming — Alberto Brandolini  
* [Alberto Brandolini](https://twitter.com/ziobrando)  

## Contributors

Thanks to all [existing and future contributors](https://github.com/ddd-crew/eventstorming-glossary-cheat-sheet/graphs/contributors) and to the following individuals who have all contributed to the EventStorming Glossary and Cheat sheet:

- [Kenny Baas-Schwegler](https://github.com/baasie)
- [Chris Richardson](https://github.com/cer)

## Contributions and Feedback

The EventStorming Glossary and Cheat sheet is freely available for you to use. In addition, your feedback and ideas are welcome to improve the technique or to create alternative versions.

If you have questions you can ping us or open an [Issue](https://github.com/ddd-crew/eventstorming-glossary-cheat-sheet/issues/new/choose).

Feel free to also send us a pull request with your examples or experience reports.

[![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a [Creative Commons Attribution 4.0 International
License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg
