---
layout: post
title:  "Test Note - Distance From Means Classifier"
date:   2020-08-15
desc: "Distance From Means Classifier"
keywords: "ML,Classifier"
categories: [Probabilistic ML]
tags: [ML,Classifier]
icon: icon-html
---

Main agenda of writing this note is to check if I can write basic latex equations, include proportionate images and give refernces and tags.

Distance from Means Classifier is the most trivial and easiest to understand machine learning algorithm.

* **Goal:** Given $$N$$ labeled training examples $$\{ x_n, y_n \}$$ from two classes, say positive and negative, we want to learn a model to predict label or class $$y$$ for a new test example $$x$$.

* **Model:** Assign $$x$$ to class with closer mean (note that the same idea can be extended to more than 2 classes)

How does it look mathematically

If $$N_{+}$$ examples form positive class and $$N_{-}$$ examples form negative class, mean of each class can be written as
	
$$\begin{equation}
\mu_{+} = \frac{1}{N_{+}} \sum_{y_n = + 1} x_n \quad and \quad \mu_{-} = \frac{1}{N_{-}} \sum_{y_n = - 1} x_n
\end{equation}$$

Distances from each mean will be then:

$$\begin{equation}
|| \mu_{+} - x ||^2 = || \mu_{+} ||^2 + || x ||^2 - 2 < \mu_{+}, x > \\
|| \mu_{-} - x ||^2 = || \mu_{-} ||^2 + || x ||^2 - 2 < \mu_{-}, x >
\end{equation}$$

This is a test note, so I am leaving it just here.

<center><img src="{{ site.img_path }}/distance_from_means/hyperplane.PNG" height="20%" width="20%"></center>

<font size="1">Reference: CS771 Slides by Piyush Rai, IIT Kanpur</font>
