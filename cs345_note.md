[TOC]





---





# Lecture 01 UX

 

## User experience (UX)

1.  **Usability** (可用性)     是否快速上手/Productivity, efficiency, ease of use, learnability

2.  **Usefulness** (有用性)   能否按照设计目的去使用 Ability to use system or product to accomplish goals of work
3.  **Emotional impact** (情绪影响)  满意度 Affective component of user experience and user feelings user satisfaction 
4.  **Meaningfulness** (意义) long-term personal relationship with the product (用户使用的持久程度)



## Usability Factors 

1. **Ease of learning** - How fast can a user who has never seen the user interface before learn it sufficiently well to accomplish basic tasks?

2. **Efficiency of use** - Once an experienced user has learned to use the system, how fast can he or she accomplish tasks?
3. **Memorability** - If a user has used the system before, can he or she remember enough to use it effectively the next time or does the user have to start over again learning everything?
4. **Error frequency**  How often do users make errors while using the system, how serious are these errors, and how do users recover from these errors?
5. **Subjective satisfaction**  How much does the user like using the system?

 

 

![image-20240329180515159](./cs345_note.assets/image-20240329180515159.png)

<center> <strong>The UX design lifecycle </strong> </center>

Understand user -> create design concepts -> realize design alternatives -> verify and refine 

 

**slip VS mistake**

- **slip** – redesign interface to make task easier to execute 

- **mistake** – need to help the user better understand the system



## Types of Usability Evaluations

* Performance measurements 

* Heuristic evaluations 

* Usability studies 

* Comparative studies (advanced class COMPSCI 705)



***



# Lecture 02 Design Walkthrough

## **Heuristic evaluation**

### Nielsen’s Heuristics

##### Background

- ​	&nbsp;  *In collaboration with Rolf Molich, Jakob Nielsen, developed a set of 10 heuristics for interface design (1990-1994).*

- ​	&nbsp;  The revised set is based on an analysis of 249 usability problems*. 

##### Principle

1. **Visibility of System Status**

​	 对**系统状态**具有可见性

2. **Match between the System and the Real World**

​	 系统和现实的匹配（比如 用 垃圾桶 来做 回收站 的图标 

3. **User Control and Freedom**

​	 用户操作的自由度（给用户 撤回undo/ redo的机会

4. **Consistency and Standards**

   内部一致性 外部分一致性（行业习惯）

   * Follow platform conventions 

   * Terminology stays constant

5. **Error Prevention**

​	 错误防御（没有填写密码不能点确定按钮 / 弹窗再次提醒）

6. **Recognition Rather Than Recall**

​	 减少用户需要记忆的内容

7. **Flexibility and Efficiency of Use**

​	 灵活性和效率（考虑**新老用户**）

8. **Aesthetic and Minimalist Design**

 	美学简约（视觉） e.g. 突出

9. **Help Users to Recognise, Diagnose, and Recover from Errors**

​	提供清晰的错误反馈，具体指导用户如何诊断并从错误中恢复，从而提高用户体验。

10. **Help and Documentation**

​	 Easy to search(Fuzzy search), focussed on the task, details concrete steps to carry out



 

## Personas, Fitts’ Law, The Human

 

 

### Conceptual Design – User Personas

 

Advantages of User Personas:

·    **Quick and Easy Creation:** Personas can be developed rapidly and without significant resources, making them an accessible tool for projects of all sizes.

·    **Consistent Reference for Teams:** They provide a uniform model of the target user for all team members, ensuring everyone works towards the same user understanding.

·    **Compatibility with Design Methods**: Personas can be easily integrated into various design processes, enhancing the design strategy with user-centered insights.

·    **Enhancing Designer Empathy**: By making the user "real" in the designer's mind, personas serve as a foundation for empathy, ensuring a user-focused approach in design decisions.

Disadvantages of User Personas:

·    **Challenges with Diversity:** Crafting personas that accurately represent an international or otherwise diverse audience can be complex and time-consuming. 

·    **Difficulty Managing Multiple Personas**: Juggling too many personas (beyond the usual 6-8) can complicate the design process, making it hard to address each persona's needs effectively.

·    **Risk of Assumption-Based Errors:** There's a potential risk that personas might include biases or unsupported assumptions by the designer, which could lead to misaligned design strategies.

 



### Conceptual Design – Scenarios

**Scenarios - Overview**

- **Definition**: Scenarios are narratives that describe a typical task a user     might perform. They are written in "plain English" to be easily     understandable.
- **Components**:
  - **Basic Goal**: The primary objective the user aims to achieve with the task.
  - **Initial Conditions**: The state of things at the beginning of the      task, providing context for the scenario.
  - **Activities**: Detailed actions the persona engages in to achieve their goal.
  - **Outcomes**: The result of the activities, indicating whether and how the      goal was achieved.

**Integration with PACT**

Scenarios are often paired with a persona to give a face to the user involved in the scenario. To further refine the scenario, it's aligned with the PACT (People, Activities, Context, Technology) structure, which considers:

- **P****eople**: Who is the persona? This includes their     characteristics that might affect how they interact with the technology.
- **A****ctivities**: What is the persona trying to accomplish?     This includes the tasks they undertake and the goals they aim to achieve.
- **C****ontext**: Where and under what circumstances is the     persona operating? This includes both physical and social contexts that     might influence their interaction.
- **T****echnology**: What tools or technologies is the persona     using to complete their activities? This considers the capabilities and     limitations of the technology in use.

 

### Summary

Personas represent archetypal users 

Scenarios capture typical tasks for a persona to be applied to

 

 

## **Fitts’ Law**

 

### $\left( T \right)$  Fitts’ Law is the classic performance measure.

* a & b are constants 
* W target width 
* D distance to move pointer 

​		$T= a + b\;log_2 \frac{2D}{W}$

​		$W = \frac{D}{2^\frac{T-1}{b}}$​



###  $\left( ID  \right)$ The $ log_2$ component is the Index of Difficulty

 		$ID = log_2 \frac{2D}{W}$

 











Prime pixel

​	\- Point  where the user will carry out their action

Magic pixels

​	\- **Four corners** of the screen (for mouse movement)

Influences

​	\- Short dropdown lists

​	\- Right-click pop-up menu

​	\- Pie menu rather than dropdown list

​	\- Large targets

Increase size until the error rate drops off

​	\- Add labels to icons

​	\- Related targets close together

 		E.g., Submit button close to last form element

​	\- Minimise distance from the attention area

 

## Hick–Hyman Law

The time it takes for a person to make a decision as a result of the **n possible choices.**

 Particularly important for menus

\- Although log2 only holds if menu is sorted in a logical order (e.g. alphabetical) – otherwise search time is linear!

\- Other factors

Recognition time: for icon or word

 

## Fitts’ Law VS Hick-Hyman Law

Fitts’ Law describes time to point at a target 

Hick-Hyman Law describes time to make a selection



---

# Week 03 Contextual Inquiry

​	\- User-Centered Scenario Investigation
​	\- 以用户为中心的情景调查

## Data Elicitation

### Conduct a field visit to the customer.

  **Observe** and interview people while they use the existing product or system

·    Write research data notes as you encounter research data points

·    Gather artefacts associated with the work practice

·    **Make sketches,** diagrams, or photos of the product or system in its physical environment



 

#### Requirements collection processes

During the collection phase you will formally identify:

\- People involved

\- Things they use

\- Processes involved

\- Information required

\- Constraints imposed

 

You will then model the information by:

\- Creating descriptions of the people who do the work

\- Documenting the main use-cases

\- Creating different stories about how the various aspects of the work are done

\- Creating formal diagrams of the interaction

 

### Collection – Elicitation Direct Interviews/ Focus Groups/ Indirect - Questionnaires:

 

**Collection - Elicitation - Direct - Interviews:**

- **On-site interviews** help in recalling     job-specific details by being in the relevant environment, enhancing     memory recall of job tasks.
- **Away from job site     interviews** ensure there are no work-related interruptions, allowing for a     focused discussion.



**Collection - Elicitation - Direct - Focus Groups:**

- Require a moderator to keep discussions relevant.
- Aim for spontaneity and clear outcomes.
- Participants should share similar backgrounds or roles.
- Separate groups for different levels (e.g., line workers and supervisors) to ensure open     communication.

**Advantages of Focus Groups:**

·    Cost-effective and straightforward to organize.

·    Useful early in the design process for feature identification and prioritization.

·    Offer insights into attitudes and motivations.

·    Highlight outlier opinions.

·    Can aid in marketing a new solution.

**Disadvantages of Focus Groups:**

·    May only reflect the views of a specific group.

·    Risk of domination by vocal participants.

·    Findings are not statistically significant.

·    Lack of usability feedback.

**Collection - Elicitation - Indirect:**

·    **Corporate Documentation:** Policies, procedures, and any formal documents that outline company practices.

·    **Logs and Notes:** Encouraging the logging of activities and collecting physical or digital notes can reveal informal practices and reminders.

**Collection - Elicitation - Indirect - Questionnaires:**

- Familiar to most     people and can include various types of questions (open, closed, scales,     choices) to gather a broad range of data.

**Advantages of Questionnaires:**

1. **Remote Administration:** Questionnaires can be     distributed and completed without the need for in-person interaction,     making it convenient to collect information from a distance.
2. **Stakeholder Profiling:** They help gather data     to create profiles for primary stakeholders to understand their needs and     preferences.
3. **Solution Validation:** They are useful for     gauging acceptance of proposed solutions and for generating new ideas.
4. **Confirmatory Tool:** They can verify     insights gathered from interviews to ensure consistency and reliability of     data.
5. **Wide Reach:** Questionnaires can be     distributed to a large number of people quickly and inexpensively.

**Disadvantages of Questionnaires:**

1. **Ambiguity:** Poorly crafted     questions may yield unclear responses that don't contribute meaningfully     to the design or understanding of the problem.
2. **Length:** People may be     reluctant to complete long questionnaires, leading to low response rates     or incomplete data.
3. **Limiting:** Closed-ended     questions can restrict the depth of responses, potentially overlooking     nuanced information.
4. **Difficult to Analyze:** Responses to     open-ended questions can be rich in detail but harder to quantify and     systematically analyze.

**Preparation Prior to the Visit:**

1. **Data Elicitation Team:** Organize a team     responsible for gathering information.
2. **Recruit Participants:**
   - Collaborate with the      client for recruitment help.
   - For consumer      products, recruit participants from the local area to get a sense of      local market needs.
   - Ensure there is a      good representation of various work roles to cover different      perspectives.
3. **Study Setting:** Identify an     appropriate setting for the study that reflects the natural work     environment of the participants.
4. **Unbiased Observation:** Observe users in     their context without managerial influence to ensure genuine behavior and     responses.
5. **Initial Questions:** Prepare initial     questions that are open-ended to encourage detailed responses and to     understand the broader context of users' experiences and needs.

 

 

 

 

Organizing the Discovery Process

 

Filters

\- **Physical** Describe the physical aspects of the activity.

\- **Cultural** Relationships among the people involved. 

\- **Functional** What actually happens.

\- **Informational** Information that is involved.

 

## Data Analysis: Affinity Diagrams

 

Arrange and process data

 

1. 确定课题 
2. 组成小组 
3. 收集资料 
4. 生成便签 
5. 分组整理便签(cetegory group)
6. 制作标签卡片
7. 作图 

 

## Ideation and Sketching



### Generative design

**Ideation **

\- Spawning ideas 

 Sketching

\- Capturing ideas

Critiquing 

\- Analysing design ideas 

Refining

\- Adopting, modifying or discarding ideas





---

# Lecture 04 Visual design

## Gestalt Principles of Perception

***Gestalt psychology** strives to explain the factors involved in the way we group things*

*At the heart **of Gestalt psychology** is the idea that we strive to find the simplest solutions to incomplete visual information **不完整的视觉信息 **(Prägnanz)*

 

### Gestalt perception is seen as based in a set of principles:

 

1. **Proximity** 

   Gestalt perception is seen as based on a set of principles:

​		*e.g. like two target **closeness***

2. **Similarity
   
   ** Objects that have similar visual characteristics, such as **size, shape** or **color** will be seen as a group and therefore related

3. **Common Fate 
   
   ** Objects that ‘move’ together (sharing a beginning and/or a direction and/or an end) are seen as related

4. **Closure

   We tend to see things as complete objects even though there may **be gaps in the shape** of the objects. （简笔画/认为一对括号是一个整体 ）

5. **Continuity**
   We tend to see things as smooth, continuous representations rather than abrupt changes

6. Area** (also called the **smallness** principle)
   Objects with small area tend to be seen as the figure, not the ground (also called the smallness principle) 
   把图像中较小的部分被认为是主体，其他部分认为是背景

7. **Symmetry **
   Symmetrical figures tend to be seen as complete figures that form around their middle

8. **Surroundedness **

   An area that is surrounded will be seen as the figure and the area that surrounds will be seen as the ground （给包围的东西被认为是正文 比如一个圆形，在一个正方形内，圆形是正文，正方形是背景）

9. **Prägnanz** （As an overarching principle**）

   we tend to perceive things based on the simplest and most stable or complete interpretation. 

### Design Principles

Principles of design are concepts used to organize or arrange the components in a design

We are going to review **3 principles**:

#### Balance

The distribution of the optical weight in an interface

* ​	&nbsp;Larger objects.

- ​	&nbsp;Cluster of small objects

* ​	&nbsp;Objects with strong, intense colors.

 

The balance in screen design is achieved by providing an equal ‘weight’ of screen elements, left and right, top and bottom.

- &nbsp;**Symmetry** ( Also called **formal balance because a form (formula) is used** )

- &nbsp;**Asymmet** **Used if two or more fundamentally different parts have to be balanced.ry** (- Also known as **informal balance.)**

Used if two or more fundamentally different parts have to be balanced.

#### Emphasis

Emphasis as a principle asks for an easily recognizable focu on color size position

#### Unity

All parts of our design have some commonality so that they are perceived as a whole

## Interaction Design

### Storyboards



* Express proposed or imagined scenarios/situations § Used throughout design in various ways
  - As a basis for overall design

  - Concrete examples of tasks


* Shows wider context and interaction from different perspectives



### Design considerations: 

**periphery** (边缘) and **focus **（焦点）, glanceable content

*重要的信息放在焦点（比如中心） 不太重要的信息放在边缘*

​	*e.g. 仪表盘把 速度 和 转速 放在仪表盘的中心 把 气温等其他不重要信息放在四周*



# Week 05 Prototyping with **Figma**

## High Fidelity Protying 