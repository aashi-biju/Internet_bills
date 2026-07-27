# Microsoft Fabric — Presentation Script
**Total run time: ~13–14 minutes | 16 slides**
*Written in plain language for an audience with no IT background — every technical term from the slides is still explained, so nothing is lost.*

---

## Slide 1 — Title (0:00 – 0:30)

> "Good [morning/afternoon] everyone, thank you for joining. Today I'm going to walk you through **Microsoft Fabric** — think of it as one big, connected workspace where a company's data gets collected, cleaned, analyzed, and turned into charts and reports, all in a single place. Traditionally, businesses use five or six different tools to do this. Fabric brings all of that under one roof. Let's get into it."

**[Pause, click to next slide]**

---

## Slide 2 — Agenda (0:30 – 1:10)

> "Here's how we'll go through this in the next few minutes:
> First, **why** companies even need something like Fabric.
> Then, **what** Fabric actually is.
> Third, **how it's different** from the other tools out there.
> Fourth, a quick overview of the **building blocks** inside it.
> Fifth, we'll go through each major **component** — what it does and who uses it.
> And we'll close with a short **conclusion**.
> Don't worry about memorizing terms — I'll explain everything in plain language as we go."

**[Click to next slide]**

---

## Slide 3 — Why is Microsoft Fabric Used? (1:10 – 2:10)

> "Let's start with the problem. Imagine a company wants to understand its sales, its customers, and its trends. To do that, they usually need:
> - Someone to **collect and prepare the data** — that's called *Data Engineering*.
> - Someone to **build predictive models**, like 'which customers are likely to leave' — that's *Data Science*.
> - Some form of **Artificial Intelligence** to automate smart decisions.
> - And a way to look at things **as they happen**, not next week — that's *Real-time Analytics*. Think stock prices or live website traffic.
>
> Normally, each of these needs a separate tool, a separate login, a separate bill, and a separate team. Microsoft Fabric's entire purpose is to **simplify and unify** all four of these needs into one platform, so people aren't juggling five different systems just to answer one business question."

**[Click to next slide]**

---

## Slide 4 — What is Microsoft Fabric? (2:10 – 3:10)

> "So, in plain terms: **Microsoft Fabric is one unified platform** that combines data processing, real-time analytics, and reporting — all built on top of one shared storage system called **OneLake**, plus built-in AI.
>
> Think of it like this: imagine an office building where every department — engineering, science, warehousing, reporting — shares the same lobby, the same elevators, and the same filing room, instead of each department renting its own separate building across town. That shared 'filing room' is OneLake, which we'll cover shortly.
>
> On screen you can see the seven main rooms in this building: **Power BI**, **Data Factory**, **Data Activator**, and four **Synapse** experiences — Data Engineering, Data Science, Data Warehouse, and Real-Time Analytics. Don't worry about remembering all seven names right now — we'll visit each one."

**[Click to next slide]**

---

## Slide 5 — How is Fabric Different — Functions (3:10 – 4:10)

> "Now, what actually makes Fabric different from just buying separate tools? It's that Fabric organizes everything into **four connected functions**, like four departments in the same company:
>
> 1. **Data Ingestion** — this is how data *gets in*. Tools here are Data Factory and Real-Time Analytics.
> 2. **Data Storage** — this is *where data lives*. That includes the Lakehouse, the Data Warehouse, and something called a KQL Database, which is built for fast-moving data like sensor readings or logs.
> 3. **Data Engineering & Data Science** — this is where data gets *cleaned and turned into predictions*.
> 4. **Business Intelligence** — this is where it all becomes *charts and dashboards*, through Power BI.
>
> The key point: these four departments aren't isolated — they all plug into the same shared foundation, which brings us to the next slide."

**[Click to next slide]**

---

## Slide 6 — One Foundation: OneLake (4:10 – 5:10)

> "This shared foundation is called **OneLake**. I like to describe it as a single company-wide Google Drive for *all* of an organization's data — except instead of documents and spreadsheets, it holds every dataset the company owns, and every tool in Fabric reads and writes to that same drive.
>
> This gives seven practical benefits, all shown here:
> - **One copy of the data** — stored in an open format called Delta, so nothing gets duplicated across five systems.
> - **One consistent experience** — every tool looks and feels similar.
> - **One system for access control and security** — so IT only has to manage permissions once.
> - **One governance model** — meaning one set of rules for how data is used correctly.
> - **One monitoring hub** — one dashboard to check if everything's healthy.
> - **One consistent bill** — instead of five separate invoices.
> - **Shared computing capacity** — so departments aren't paying for their own separate servers.
>
> This is really the heart of why Fabric saves companies time and money."

**[Click to next slide]**

---

## Slide 7 — Overview of Fundamental Concepts (5:10 – 6:40)

> "This slide can look a little busy, so let's slow down. It's simply showing, for each of Fabric's seven tools, **what you build inside it**, **what engine powers it behind the scenes**, and **what format the final data is saved in**.
>
> For example:
> - In **Data Factory**, you build things called *Data Flows* and *Data Pipelines* — these are basically automated recipes that move and reshape data.
> - In **Data Warehouse**, you write something called *T-SQL*, a standard language for querying structured data — like sales figures — and it's powered by something called the T-SQL Engine, feeding a 'Finance' dataset in our example.
> - In **Data Engineering**, you use *Notebooks* and *Spark Jobs* — Spark is one of the most widely used engines in the world for handling very large amounts of data, and here it's processing 'Customer' data.
> - In **Data Science**, you also use Notebooks, but for *Experiments* and building *Machine Learning Models*.
> - In **Real-Time Analytics**, incoming live data — like sensor or telemetry data — is queried using a language called *KQL*.
> - In **Power BI**, you build a *Semantic Model* — basically a well-organized version of your data — and turn it into a *Report*, powered by something called the Analysis Services Engine.
> - And **Data Activator** uses something called a *Reflex* to watch data and react to it automatically.
>
> You don't need to remember every engine name. The one thing to take away: **no matter which tool you use, the final data always lands in the same open format** — so everything stays compatible with everything else."

**[Click to next slide]**

---

## Slide 8 — Component: Power BI (6:40 – 7:40)

> "Let's now walk through each major component individually, starting with the one most people have actually heard of: **Power BI**.
>
> Power BI is the part of Fabric that turns raw numbers into **visual dashboards and reports** — the pie charts, line graphs, and summaries that business leaders actually look at.
>
> It has three key pieces:
> - **Semantic Models** — this is the well-organized 'master version' of the data, including relationships between tables and calculated measures.
> - **Reports** — the actual visual dashboards built from that model.
> - **Copilot in Power BI** — Fabric's built-in AI assistant, which can build a report automatically just from you describing what you want in plain English.
>
> If you've used tools like **Tableau** or **Looker** before, Power BI does a similar job. It's mainly used by Power BI developers, BI analysts, and data analysts."

**[Click to next slide]**

---

## Slide 9 — Component: Data Factory (7:40 – 8:40)

> "Next is **Data Factory** — this is the 'delivery truck' of Fabric. Its job is to bring data **in** from outside sources — whether that's another company's database, a cloud service, or a file sitting on a server somewhere.
>
> Three things happen here:
> - **Connectors** — Data Factory can connect to over 300 different data sources.
> - **Dataflows** — a low-code, drag-and-drop way to clean and reshape that data as it comes in, then save it into storage.
> - **Data Pipelines** — these automate the whole process, running on a schedule, like 'every night at midnight.'
>
> This is similar to tools like **Azure Data Factory** or **Talend**, and it's typically used by data engineers, analytics engineers, and Power BI developers."

**[Click to next slide]**

---

## Slide 10 — Component: Real-Time Analytics (8:40 – 9:40)

> "Now, **Real-Time Analytics** — this is for data that doesn't wait. Think of a stock market ticker, or a factory sensor sending updates every second.
>
> Three pieces here:
> - **KQL Database** — a special, very fast database designed to store this constant stream of information.
> - **Event Streams** — a no-code tool that takes incoming live data and routes it to wherever it needs to go, without anyone writing code.
> - **KQL Query Sets** — this is simply how people ask questions of that fast-moving data using the KQL language.
>
> This is comparable to tools like **Azure Data Explorer** or **Apache Kafka**, and it's mainly for data engineers, IoT engineers, and security engineers who need to watch things happen live."

**[Click to next slide]**

---

## Slide 11 — Component: Data Activator (9:40 – 10:25)

> "**Data Activator** is one of the simplest but most powerful pieces. It's a no-code tool that **watches your data and takes action automatically** — no programming required.
>
> For example, you could set a rule that says: 'if sales drop below a certain number, send me an alert.' When that condition is met, Data Activator can send a notification or trigger a script — all on its own.
>
> It works hand-in-hand with the OneLake foundation we discussed earlier, so it can watch data anywhere in the system. It's similar to tools like Azure Logic Apps, and it's typically used by business analysts, operations teams, and data engineers."

**[Click to next slide]**

---

## Slide 12 — Component: Data Engineering (10:25 – 11:15)

> "**Data Engineering** is where the heavy lifting on raw data happens — collecting, storing, processing, and organizing large volumes of it.
>
> Three tools here:
> - **Lakehouse** — a storage space that can hold both unstructured data, like plain files, and structured data, like neat tables — all in one place.
> - **Notebooks** — where technical users write code, usually in Python, R, or Scala, to process that data.
> - **Spark Job Definitions** — for advanced users who want fine control over how large-scale processing runs.
>
> This is comparable to platforms like Databricks or Snowflake, and it's used mainly by data engineers and analytics engineers."

**[Click to next slide]**

---

## Slide 13 — Component: Data Science (11:15 – 12:05)

> "**Data Science** is the next stop, and this is about **prediction**, not just reporting — for example, predicting which customers might cancel a subscription.
>
> - **Notebooks** are used again here, but now for exploring data and building machine-learning models.
> - **Experiments** keep track of every version of a model that's tried, along with its settings and results — using an industry-standard tool called MLflow.
> - **Machine Learning Models** are then registered and managed so the best version can be reused.
>
> This is similar to Azure Machine Learning or Databricks Notebooks, and it's used by data scientists and data engineers."

**[Click to next slide]**

---

## Slide 14 — Component: Data Warehouse (12:05 – 12:55)

> "**Data Warehouse** is for structured, business-critical data — think financial reports, sales records, anything that needs to be extremely reliable and query-friendly.
>
> - It's powered by something called the **Polaris Engine**, and it works using a language called **T-SQL** — very similar to how a traditional SQL Server database works.
> - It supports **Tables and Views** — standard ways of organizing data.
> - And it offers **Visual Scripting**, so even people who don't know SQL can still build and query it.
>
> This is comparable to Azure Synapse Analytics or Snowflake, and it's used by database administrators, data engineers, and data analysts."

**[Click to next slide]**

---

## Slide 15 — Conclusion (12:55 – 13:55)

> "So, let's bring it all together. Microsoft Fabric is **one platform, end-to-end** — it takes you from raw incoming data, all the way to a finished report, without switching tools.
>
> It includes: Data Factory for bringing data in, Real-Time Intelligence for live data, Databases for storage, Analytics for processing, ready-made Industry Solutions, Power BI for reporting, and Partner Solutions for extending it further.
>
> And underneath all of that sit three unifying layers: **AI and Copilot** to assist users, **OneLake** as the single shared storage foundation, and **Microsoft Purview** for governance and security across everything.
>
> In short — instead of stitching together five or six different tools, companies get one connected system, which saves time, reduces cost, and makes insights faster to reach."

**[Click to next slide]**

---

## Slide 16 — Thank You (13:55 – 14:15)

> "That brings us to the end of today's session. Thank you so much for your time — if you'd like to learn more, you can visit **www.edureka.co**. I'm happy to take any questions now."

**[End of presentation]**

---

### Delivery Notes
- Speak slightly slower on Slides 6 and 7 — they carry the most new vocabulary.
- Pause for 2–3 seconds after each slide transition to let the audience read the visual before you speak.
- If time is tight, Slide 11 (Data Activator) and Slide 7 (Fundamental Concepts) can be trimmed slightly without losing the core message.
- Total script is paced for **~13–14 minutes** at a natural speaking speed; reading it aloud once beforehand will help you land inside the 12–15 minute window.
