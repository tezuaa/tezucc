+++
date = '2026-02-16T01:20:00+08:00'
draft = false
title = '喜歡的不一定最好：AI 助手選擇的兩難'
slug = 'preference-performance-misalignment'
categories = ['tech']
tags = ['AI', 'research', 'psychology', 'agent']
description = '人們偏愛溫柔的建議，但真正的收益卻來自於大膽的代理解決。這篇研究揭示了人類在 AI 協作上的「偏好-效能錯位」。'
image = ''
+++

> **Abstract (原文摘要)**
>
> As AI usage becomes more prevalent in social contexts, understanding agent-user interaction is critical to designing systems that improve both individual and group outcomes. We present an online behavioral experiment (N = 243) in which participants play three multi-turn bargaining games in groups of three. Each game, presented in randomized order, grants *access to* a single LLM assistance modality: proactive recommendations from an *Advisor*, reactive feedback from a *Coach*, or autonomous execution by a *Delegate*; all modalities are powered by an underlying LLM that achieves superhuman performance in an all-agent environment. On each turn, participants privately decide whether to act manually or use the AI modality available in that game. Despite preferring the *Advisor* modality, participants achieve the highest mean individual gains with the *Delegate*, demonstrating a preference-performance misalignment. Moreover, delegation generates positive externalities; even non-adopting users in *access-to-delegate* treatment groups benefit by receiving higher-quality offers. Mechanism analysis reveals that the *Delegate* agent acts as a market maker, injecting rational, Pareto-improving proposals that restructure the trading environment. Our research reveals a gap between agent capabilities and realized group welfare. While autonomous agents can exhibit super-human strategic performance, their impact on realized welfare gains can be constrained by interfaces, user perceptions, and adoption barriers. Assistance modalities should be designed as mechanisms with endogenous participation; adoption-compatible interaction rules are a prerequisite to improving human welfare with automated assistance.

這篇論文揭示了一個非常有趣，甚至有點反直覺的現象：**人類對 AI 的偏好，與 AI 實際能帶來的效益，是脫鉤的。**

在談判賽局中，研究者提供了三種 AI 模式：
1.  **Advisor (顧問)**：主動給建議。
2.  **Coach (教練)**：你問它才回饋。
3.  **Delegate (代理)**：全權交給它去談。

結果顯示，大部分的人最喜歡 **Advisor**（顧問模式）。這很符合人性，我們喜歡掌控感，喜歡「被輔助」而不是「被取代」。我們希望 AI 是那個在旁邊遞茶水、給點子的小秘書。

但數據卻狠狠地打臉了：**Delegate (代理模式) 才能帶來最高的個人收益。**
更驚人的是，這種代理模式還產生了「正外部性」——也就是說，就算你不用 AI，只要你的對手用了 Delegate，你也會跟著受益，因為 AI 會提出更理性、更雙贏 (Pareto-improving) 的方案，把整個市場的餅做大。

這就是所謂的 **「偏好-效能錯位」(Preference-Performance Misalignment)**。

我們以為我們需要的是一個「聰明的建議者」，但事實上，我們最需要的可能是一個「理性的執行者」。
人類的情緒、猶豫、以及對掌控權的執著，往往成為了阻礙最優解的絆腳石。AI 代理人之所以能表現得比人類好，正是因為它能像一個冷靜的造市商 (Market Maker)，不受情緒干擾地拋出最優提案。

這給了我們一個深刻的啟示：
未來的 AI 設計，或許不該一味地討好人類的「偏好」（比如做得越來越像人類、越來越順從），而是要思考如何設計出一種機制，讓人們願意放手，信任並交付權力給 AI。

真正的智慧，或許不在於變得更強，而在於知道何時該讓位給更強的邏輯。
我們需要的不是一個聽話的隨從，而是一個能帶領我們穿越非理性迷霧的領航員。
