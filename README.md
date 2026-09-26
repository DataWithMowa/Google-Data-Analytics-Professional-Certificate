# Google-Data-Analytics-Professional-Certificate
Google Data Analytics Professional Certificate completed through the Wetech Inc Data Analytics Track. Developed practical skills in data cleaning, analysis, visualization, spreadsheets, SQL, Tableau, and Python through hands-on projects, assessments, and a real-world case study.

Tools Learnt;
- Google Sheet
- --Sorting, Formulars, Data Entry, Data visulaization
- SQL

One of the major things I've learned so far in this course is fairness in data analytics, meaning there should be no reinforce bias in the analytics process

Absolutely. Think of **fairness in data analytics** as:

> **“Don’t let the data or the way you analyze it unfairly disadvantage a particular group of people.”**

And importantly, **fairness doesn't mean treating every group exactly the same.** Sometimes different groups need to be considered differently because the underlying circumstances are different.

### A simple case study: Bank loan approval

Imagine a bank wants to use data to predict who is likely to repay a loan.

They collect:

* Income
* Age
* Employment history
* Credit history
* Previous repayments
* Location
* Loan amount

The analyst discovers something:

> People from Area X have historically defaulted on loans more often.

The bank then creates a rule:

> **“Applicants from Area X should have a lower chance of getting approved.”**

At first, this might look like a data-driven decision.

But there's a problem.

### Where does bias enter?

Maybe Area X has historically had:

* fewer formal employment opportunities
* poorer access to banking
* lower average incomes
* fewer credit-reporting records

So the **location itself isn't necessarily causing someone to be a bad borrower.**

If we use that historical pattern without thinking about why it exists, our model could simply reproduce an existing disadvantage.

That's called **reinforcing bias**.

### Another example

Suppose historical loan data shows:

| Group   | Approval rate |
| ------- | ------------: |
| Group A |           70% |
| Group B |           45% |

An analyst shouldn't immediately conclude:

> “Group B is riskier.”

They should ask:

**Why?**

Maybe the historical approval process itself was biased.

So if we train a machine-learning model on those historical decisions, the model may learn:

> “People like Group B should be rejected more often.”

The model isn't necessarily being intentionally unfair.

**It is learning the unfairness contained in the historical data.**

### What should the analyst do?

A good analyst should:

**1. Look for patterns across groups**

Don't only look at the overall average.

Break results down by relevant groups and check whether the conclusions change.

**2. Question the data**

Ask:

> “How was this data collected?”

> “Could historical decisions already contain bias?”

> “Are some groups underrepresented?”

**3. Don't use sensitive characteristics carelessly**

Things such as gender, ethnicity, religion, disability, etc. can create serious fairness concerns depending on the use case and jurisdiction.

Even removing such a column doesn't automatically solve the problem. Other variables can sometimes act as **proxies** for it.

**4. Check the outcome after building the model**

If a model is being used for an important decision, compare its performance across groups.

For example:

> Does the model make significantly more false rejections for one group?

That is something worth investigating.

---

### The principle I want you to remember

**Data can be accurate and still produce an unfair outcome.**

That's why a good data analyst doesn't only ask:

> **“What does the data say?”**

They also ask:

> **“How was this data produced, who might be affected, and could my analysis reinforce an existing unfairness?”**

That is one of the differences between **just analyzing data** and practicing **responsible data analytics**.

Yes. Your practice questions actually point to a **very useful way of thinking about fairness**. The big idea is that fairness is not something you check only after you finish analyzing the data.

### The simple definition

**Fairness in data analytics means making sure your data, analysis, and conclusions do not unfairly favor or disadvantage a group of people.**

And there are several practical ways to do that.

### 1. Consider fairness from beginning to conclusion

Don't wait until the dashboard is finished.

Think about fairness when you:

**Plan → Collect → Process → Analyze → Share/Present**

For example, if you're analyzing customer satisfaction, ask from the beginning:

> “Whose experiences are represented in this data, and whose might be missing?”

---

### 2. Consider the surrounding factors

This is probably one of the most important lessons.

**A pattern in data doesn't automatically explain why the pattern exists.**

Remember the ballet example:

> 85% of dancers are under 34.

You could conclude:

> “Young people are more likely to succeed.”

But that's not necessarily true.

Maybe younger people are simply the people who have historically been given more opportunities.

So instead of immediately acting on the number, investigate the **surrounding factors**.

This is basically asking:

> **“What else could be causing this result?”**

That's excellent analytical thinking too.

---

### 3. Consider all relevant data

Don't build your conclusion from one narrow piece of information.

Imagine a hospital wants to understand low blood pressure.

Looking only at blood-pressure readings gives you one part of the story.

But adding:

* Age
* Medical history
* Lifestyle
* Medication
* Other demographics
* Relevant environmental factors

can give you a much better understanding.

**More relevant context → better analysis.**

---

### 4. Use self-reported data when appropriate

Sometimes the people experiencing something are the best source of information about their experience.

For example, a library wants to know whether users feel welcome.

Instead of relying entirely on librarians' observations, the library could ask **the users themselves**.

Why?

Because the librarian's observation could unintentionally contain their own assumptions.

Self-reported information doesn't automatically remove bias, but it can provide an important perspective that would otherwise be missing.

---

### 5. Use oversampling when a group is underrepresented

This one is interesting.

Suppose you survey 1,000 people:

* 900 have already voted
* 100 haven't voted

If you want to understand the views of people who **haven't voted**, their experiences could get drowned out by the much larger group.

Oversampling means deliberately collecting more responses from the underrepresented group.

You're essentially saying:

> **“This group is too small in our dataset, so let's make sure we hear from them properly.”**

It doesn't mean pretending the group is larger than it really is. It helps you collect enough information to analyze that group meaningfully.

---

### 6. Don't confuse correlation with explanation

This connects everything together.

Suppose your analysis says:

> Customers in Region A spend less money.

Don't immediately say:

> “Customers in Region A are less valuable.”

Instead ask:

* Are there fewer customers there?
* Are certain products unavailable?
* Are prices different?
* Is income different?
* Is delivery more expensive?
* Is the sample representative?
* Are there other factors?

**The number tells you WHAT happened.
Good analysis investigates WHY.**

---

## The fairness checklist I'd remember

When you're working on your own projects, remember these **5 questions**:

**1. Who is represented?**
Who is actually in my data?

**2. Who is missing?**
Could an important group be underrepresented?

**3. What other factors matter?**
Am I looking at the full context?

**4. Could my data contain existing bias?**
Was the data collected fairly?

**5. Could my conclusion disadvantage someone?**
Am I turning a pattern into an assumption?

That's the heart of **fair and ethical data analytics**.

And honestly, this connects beautifully with the kind of analyst you're trying to become: **don't just make the chart look good—question what the numbers actually mean.**

Today, I learnt that a good data analyst doesn't only ask:

> **“What does the data say?”**

They also ask:

> **“How was this data produced, who might be affected, and could my analysis reinforce an existing unfairness?”**

That is one of the differences between **just analyzing data** and practicing **responsible data analytics.**

I learnt that fairness should be considered from the **beginning to the end** of an analysis.

Some simple best practices are:

• Consider the surrounding factors
• Look at all relevant data
• Watch out for bias in existing data
• Include underrepresented groups
• Use self-reported data when appropriate

**Data can show you a pattern, but context helps you understand what that pattern really means.**

For example, if data shows that 85% of successful ballet dancers are under 34, it would be easy to conclude that younger people are more likely to succeed.

But a good analyst should pause and ask:

Why?

Could there be other factors behind that pattern?

The data may show a relationship, but understanding the context behind the relationship is where good analysis begins.

Another lesson for me:

Data can be accurate and still lead to an unfair conclusion.

