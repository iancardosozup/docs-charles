---
title: Key concepts
weight: 2
description: >-
  In this section, you will find the definitions of the main concepts and
  expressions used on Charles' platform and documentation.
---

---

## **Circles**

**Circles** are groups of users created from specific characteristics, inside the same environment on Charles' platform. The developer is able to segment users according to the rules "AND/OR" which will make more sense to test that release later.

For example, it is possible to [**create a circle**]({{< ref path="/Reference/Circles.md" lang="en">}}) of engineers from the north of Brazil, another one from the southeast, and the third one with all Brazilian engineers. Based on the client's segmentation, it is possible to make a variety of deployment logic.

## **Circle Matcher**

It is an HTTP service that allows you to identify which segmentation the user belongs to, based on predefined logic rules. For that, Circle Matcher receives a JSON request with the user's attributes and also the circle identifier of which group user belongs.

## **Components**

Components are part of the [**modules**]({{< ref path="/Get Started/Creating your first module/Overview.md" lang="en">}}) you create on Charles. They work as an application abstraction, which means that they have their own configuration and every part of it belongs to a module application you are working on it.

## **Open Sea**

This term was originated with Charles and refers to a default segmentation that will be used for all users not linked to any circle.

For example, if you add 300 users to your database and don't specify which segmentation you want to direct your hypothesis, Charles will redirect it to all, that is when your hypothesis will fall into the open sea.

## **Modules**

The module is a representation of your git repository. Besides that, a module can have one or more applications, which means one or more components.
