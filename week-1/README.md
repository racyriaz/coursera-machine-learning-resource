# Machine Learning - Defination

* Arthur Samuel - a checker board game designer from 1950's defined the term ML as (old ML defination)
  * ML is a feild of study that gives computers **the ability to learn without being explicitly programmed.**

* Tom Mitchell a friend of Carnegie Melon says
  * A computer program is said to **learn from the Experience _(E)_ with respect to some task _(T)_ and some performance measure _(P)_.**
  * such that the performance P is directly propotional to the experience E with respect to the task.

## Major types of Machine learning

 1. [Supervised Learning](#supervised)
 2. [Unsupervised Learning](#Unsupervised-Learning)
 3. Reinforcement Learning
 4. Recommender systems

 ---

### Supervised Learning {#supervised}

  In Supervised Learning, we are given a dataset that already has the correct answer/output. The main idea will be to find the relationship between the inputs/attributes/features/X and the output(y).

* Supervised learning problem are categorized into _"regression"_ and _"classification"_ problems.

  * In **Regression**, we try to predict the results with continuous output.
  * In **Classification**, we try to predict the result in discrete output i.e. map the inputs into discrete/unique categories.

**Example 1:**

Given data about the size of houses on the real estate market, try to predict their price. Price as a function of size is a continuous output, so this is a regression problem.

We could turn this example into a classification problem by instead making our output about whether the house "sells for more or less than the asking price." Here we are classifying the houses based on price into two discrete categories.

**Example 2:**

(a) Regression - Given a picture of a person, we have to predict their age on the basis of the given picture

(b) Classification - Given a patient with a tumor, we have to predict whether the tumor is malignant or benign.

---

### Unsupervised Learning

Unsupervised Learning allows us to work on the problems that has little or no idea on what our results should look like.

* We can derive a **structure by clustering the relationship between the datas**.
* They have no feedbacks based on the prediction result.

**Example:**
**_Clustering:_** Take a collection of 1,000,000 different genes, and find a way to automatically group these genes into groups that are somehow similar or related by different variables, such as lifespan, location, roles, and so on.

**_Non-clustering:_** The "Cocktail Party Algorithm", allows you to find structure in a chaotic environment. (i.e. identifying individual voices and music from a mesh of sounds at a cocktail party).

**Applications:**

1. Market segmentations
2. Social Network Analysis (friend circle)
3. Astronomical data analysis
4. Organize computing clusters
