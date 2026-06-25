# Empirical Corporate Finance: Foundations and Applications

*A PhD-level treatment of how empirical corporate finance research is actually done, organized around a single distinction: the structural and the causal.*

Murray Z. Frank · Carlson School of Management, University of Minnesota

The book is at: https://github.com/mzfrank/ECF/blob/main/ECF_2026_May.pdf
---

## What this book is

This book grew out of the doctoral empirical corporate finance sequence at the Carlson School, taught regularly at least since 2009. This is not a survey of literatures from a distance. The aim is to help the student build judgment as they move from being a consumer of research to becoming a producer. The idea is to help smooth that path.

The materials covered are central to the empirical corporate finance literature. This book is written because there is no graduate level empirical corporate finance textbook. So over the years I wrote many handouts and teaching materials. Here I draw them together as a single coherent project. Claude Opus was very helpful both with unifying what I had and with improving the writing and generating nicely commented coding materials. This book covers what a corporate finance researcher should know about both the structural and the causal traditions and how to choose between them. That is the gap this book aims to fill. There has been variation for year to year in what topics are covered. Partly that reflects changes in the literature. As a result there are more chapters in the
book than I actually assign in class.

Every empirical paper in corporate finance is trying to recover one of a small number of objects. It may be a descriptive regularity, a prediction, a causal effect, a structural primitive, or a counterfactual. 
The object dictates the assumptions, the assumptions dictate the method, and the method determines what the estimate means. A regression coefficient is not a treatment effect. A treatment effect is not a 
structural parameter. A structural parameter is not, by itself, a claim about any observable variation. Confusing these objects is one of the most common sources of miscommunication. It is also readily 
corrected by being clear about what is being assumed. Often assumptions are left implicit, and that is a cause of considerable confusion. 

A second idea runs through the applications. The chapters on investment, financial constraints, capital structure, and payout are usually taught as separate literatures with separate canonical papers. 
This book treats them instead as connected margins of one object. It is the shadow value of internal funds, the multiplier on the firm's budget constraint in any dynamic model where external finance is 
costly. The structural tradition estimates that object and the frictions behind it. The causal tradition identifies how behavior at one margin responds when a shock moves the value of internal funds for 
some population of firms. Read through this common object, papers that look unrelated turn out to be studying different sides of the same mechanism. Where the framing organizes a literature cleanly, the 
book lets it work. Where it does not properly unify topics I do not try to fore it. 

## Who it is for

The primary reader is a PhD student in finance or economics who will use these methods in dissertation work. The book assumes a first year graduate econometrics sequence, a course in corporate finance 
theory. A working comfort with Stata or Python is important to have or to establish. In recent years students often have been taught econometrics from Cunningham, Scott. Causal inference: The mixtape. 
Yale university press, 2021. I tend to point them to Cameron, Adrian Colin and Pravin Trivedi. Microeconometrics using Stata, Second Edition. Stata Press, 2022. Previous training in corporate finance 
theory is much more varied. 

I have attempted to write in a conversational but rigorous style. This is motivated by two books that I particularly admire: Angrist, and Pischke, 2009. Mostly harmless econometrics: An empiricist's 
companion. Princeton university press; and by Cochrane, 2009. Asset pricing: Revised edition. Princeton university press. 

## How it is organized

**Part I — Frameworks.** Required reading for everyone. The structural versus causal distinction and the identification logic that follows from it are used in every later chapter.
- Structural and Causal Approaches
- Identification

**Part II — Methods.** Widely used tools, readable in order or as reference. Each connects explicitly back to Part I.
- Panel Data
- Event Studies
- Instrumental Variables
- Difference-in-Differences
- Machine Learning

**Part III — Frictions and the Shadow Value of Internal Funds.** Applications. The first four chapters study connected margins of the same object. The rest turn to other important corporate finance topics. 
Each chapter presupposes Part I but is otherwise self-contained.
- Investment
- Financial Constraints
- Capital Structure
- Payout Policy
- Banking and Credit Supply
- Innovation
- Corporate Governance
- Mergers, Acquisitions, and Restructuring

Every chapter shares the same architecture. It opens with the economic question, develops the intuition, states the formal framework, applies the method to a corporate finance setting, and closes with common 
mistakes, decision rules, exercises, and further reading.

## The running example

One relationship threads through much of the book: how firm leverage affects firm investment. It can be approached from a structural approach or from a causal approach. Both are in the literature. This topic
has been studied at length, and it returns in different methodological guises as the book progresses. It is introduced in the first chapter, given its identification treatment in the second, takes its full 
panel data form later, and reappears under instrumental variables, difference-in-differences, and then across the applications, each time on a different margin. The point of returning to one relationship through 
so many lenses is not that the estimates should agree. They recover different objects, and seeing why is the lesson.

## Reproducibility and code

The empirical work is reproducible. A master Compustat panel is being built early and augmented with CRSP, FHFA, ISS, and other sources as later chapters require them. Both Stata and Python are used. The dynamic 
simulations and structural estimation are Python only. Stata replication files are used for reduced form and causal exercises, where Stata matches common practice in the literature. A random seed of 8823 is used 
throughout, so a reader who runs the code sees the same numbers that appear in the text.

## What is in this repository

- For now: the manuscript (compiled PDF). 
- Eventually: the **Code Companion**, which collects the code in book order and is meant to be read alongside the relevant chapters.
- Eventually: the **replication archive**: the full runnable code, the data construction pipelines, and the Stata and Python replication files that produce the tables and figures.

## Scope

The book covers roughly what is taught in a PhD course titled *Empirical Corporate Finance*. It deliberately leaves out household finance, labor-market aspects, international corporate finance, the impact of 
artificial intelligence on firms, and entrepreneurial finance and venture capital. Each omission reflects a choice about scope, not a judgment about importance. Those are all wonderfully interesting and important
topics. But we cannot do everything.

## Status and feedback

This is a working draft, posted publicly while the book is being finished. Errors are inevitable in a project of this scope. If you find one, or have a suggestion, please get in touch: murra280@umn.edu.

Murray Z. Frank · Minneapolis, Minnesota
